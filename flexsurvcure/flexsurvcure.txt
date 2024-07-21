# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Flexible Parametric Survival Models with Cure Fraction for flexsurvreg Use flexsurvcure With (In) R Software
install.packages("flexsurvcure")
library("flexsurvcure")
flexsurvcure = read.csv("https://raw.githubusercontent.com/timbulwidodostp/flexsurvcure/main/flexsurvcure/flexsurvcure.csv",sep = ";")
# Estimation Flexible Parametric Survival Models with Cure Fraction for flexsurvreg Use flexsurvcure With (In) R Software
flexsurvcure_weibull <- flexsurvcure(Surv(rectime,censrec)~group, data=flexsurvcure, dist="weibull", anc=list(scale=~group))
print(flexsurvcure_weibull)
flexsurvcure_lnorm <- flexsurvcure(Surv(rectime,censrec)~group, data=flexsurvcure, dist="lnorm", mixture = FALSE)
print(flexsurvcure_lnorm)
flexsurvcure_weibull_loglog <- flexsurvcure(Surv(rectime,censrec)~group, data=flexsurvcure, dist="weibull", link="loglog")
print(flexsurvcure_weibull_loglog)
# Flexible Parametric Survival Models with Cure Fraction for flexsurvreg Use flexsurvcure With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished