# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Estimate a Dynamic Factor Model Use DFM (dfms) With (In) R Software
install.packages("dfms")
install.packages("magrittr")
install.packages("xts")
install.packages("vars")
library("magrittr")
library("xts")
library("vars")
library("dfms")
# Estimate a Dynamic Factor Model Use DFM (dfms) With (In) R Software
DFM_M = read.csv("https://raw.githubusercontent.com/timbulwidodostp/DFM_M/main/DFM_M/DFM_M.csv",sep = ";")
DFM_Q = read.csv("https://raw.githubusercontent.com/timbulwidodostp/fuzzydid/main/DFM_Q/DFM_Q.csv",sep = ";")
DFM_Models = read.csv("https://raw.githubusercontent.com/timbulwidodostp/DFM_Models/main/DFM_Models/DFM_Models.csv",sep = ";")
DFM_ = merge(DFM_M, DFM_Q)
DFM <- DFM(DFM_[, DFM_Models$small], r = 2, p = 3)
summary(DFM)
# Estimate a Dynamic Factor Model Use DFM (dfms) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished