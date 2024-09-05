# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Regresssion Design Discontinuity (RDD) parametric and nonparametric local linear Use rdd_reg_lm and rdd_reg_np (rddtools) With (In) R Software
install.packages("rddtools")
library("rddtools")
rddtools = read.csv("https://raw.githubusercontent.com/timbulwidodostp/rddtools/main/rddtools/rddtools.csv",sep = ";")
# Estimation Regresssion Design Discontinuity (RDD) parametric and nonparametric local linear Use rdd_reg_lm and rdd_reg_np (rddtools) With (In) R Software
# Regression Discontinuity Design (RDD) parametric
rddtools_rdd <- rdd_data(y=rddtools$y, x=rddtools$x, cutpoint=0)
RDD_parametric <- rdd_reg_lm(rdd_object=rddtools_rdd)
print(RDD_parametric)
summary(RDD_parametric)
# Regression Discontinuity Design (RDD) nonparametric local linear
RDD_nonparametric <- rdd_reg_np(rdd_object=rddtools_rdd)
print(RDD_nonparametric)
summary(RDD_nonparametric)
# Regresssion Design Discontinuity (RDD) parametric and nonparametric local linear Use rdd_reg_lm and rdd_reg_np (rddtools) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished