## Gatekeeper
rm(list=ls())
setwd("P:/Evaluation/TN Lives Count_Writing/3_Target1_SUICClinicalTrainingComparison/3_Data & Analyses")
datPre = read.csv("Pre.csv", header = FALSE, row.names = NULL)
datPost = read.csv("Post.csv", header = FALSE, row.names = NULL)
dat3month = read.csv("3month.csv", header  = TRUE)

#Connections
rm(list=ls())
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/ConnectionsPaperData")
GPRAAll = read.csv("ConnGPRA.csv", header = TRUE) 
PHQ9Base = read.spss("S:/Indiana Research & Evaluation/Indiana Connections/Data/PHQ9/PHQ9 Baseline.sav", to.data.frame = TRUE)
PHQ96month = read.spss("S:/Indiana Research & Evaluation/Indiana Connections/Data/PHQ9/PHQ9 6 Month.sav", to.data.frame = TRUE)
PHQ9All = merge(PHQ9Base, PHQ96month, by = "ParticipantID", all = TRUE)
GAD7Base = read.spss("S:/Indiana Research & Evaluation/Indiana Connections/Data/GAD7/GAD7 Baseline.sav", to.data.frame = TRUE)
GAD76month = read.spss("S:/Indiana Research & Evaluation/Indiana Connections/Data/GAD7/GAD7 6 Month.sav", to.data.frame = TRUE)



#BAHCS-10
rm(list=ls())
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/HealthCapitalScale/7-13-18HCSData")
CIL = read.csv("CIL HCS Dataset_07172018.csv", header = TRUE)
CKY = read.csv("CKY HCS Dataset_07172018.csv", header = TRUE)
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/HealthCapitalScale/7-13-18HCSData")
CILDemo = read.csv("Brief HCS - IL - Demographics - 20180813.csv", header = TRUE)
CKYDemo = read.csv("Brief HCS - KY - Demographics - 20180813.csv", header = TRUE)
CIL_South_HCS_tobacco_use = read.csv("CIL_South_HCS_tobacco_use.csv", header = TRUE)
CIL_West_HCS_tobacco_use = read.csv("CIL_West_HCS_tobacco_use.csv", header = TRUE)
CKY_HCS_tobacco_use = read.csv("CKY_HCS_tobacco_use.csv", header = TRUE)
CIL_South_HCS_vitals = read.csv("CIL_South_HCS_vitals.csv", header = TRUE)
CIL_West_HCS_vitals = read.csv("CIL_West_HCS_vitals.csv", header = TRUE)
CKY_HCS_Vitals = read.csv("CKY_HCS_Vitals.csv", header = TRUE)
CIL_South_HCS_PHQ9 = read.csv("CIL_South_HCS_PHQ9.csv", header = TRUE)
CIL_West_HCS_PHQ9 = read.csv("CIL_West_HCS_PHQ9.csv", header = TRUE)
CKY_HCS_PHQ9 = read.csv("CKY_HCS_PHQ9.csv", header = TRUE)
HCS = read.csv("HCS.csv", header = TRUE)


#October 2018 BACHS-10 and Passport
rm(list=ls())
setwd("T:/Clinical Model Materials/Clinical Models/Adult Health Home/Evaluation Materials/Data/1. Health Capital Scale/6. October 2018/Matt'sData")
CIL_South_HCS_10052018 = read.csv("CIL_South_HCS_10052018.csv", header = TRUE)
CIL_West_HCS_10052018 = read.csv("CIL_West_HCS_10052018.csv", header = TRUE)
CKY_HCS_10052018 = read.csv("CKY_HCS_10052018.csv", header = TRUE)
setwd("T:/PP Claims Data/Matt'sStuff")
InfoMC10_PassPort_10_18 = read.csv("InfoMC10-18.csv", header = TRUE)
CIL_CKYFull = read.csv("CIL_CKYFull10-18.csv", header = TRUE)
setwd("T:/PP Claims Data/Matt'sStuff")
Member2017 =  read.csv("MEMBER_20170809_00.csv", header = TRUE)
Member2018 = read.csv("MEMBER_20180816_00.csv", header = TRUE)
SystemIDConverter = read.csv("SYSTEM_ID_to_AvatarClient_ID_Mapping.csv", header = TRUE)
Claims2017 = read.csv("CLAIMS_20170809_00.csv", head = TRUE) 
Claims2018 = read.csv("CLAIMS_20180816_00.csv", header = TRUE)
PHARMCLAIMS_2017 = read.csv("PHARMCLAIMS_20170809_00.csv", header = TRUE)
PHARMCLAIMS_2018 = read.csv("PHARMCLAIMS_20180816_00.csv", header = TRUE)
Provider2017 = read.csv("PROVIDER_20170809_00.csv", header = TRUE)
Provider2018 = read.csv("PROVIDER_20180816_00.csv", header = TRUE)
InpatClaimsData = read.csv("InpatClaimsData.csv", header = TRUE)
InpatAvatarData = read.csv("InpatAvatarData.csv", header = TRUE)
OutpatClaimsData = read.csv("OutpatClaimsData.csv", header = TRUE)
OutpatAvatarData = read.csv("OutpatAvatarData.csv", header = TRUE)



#Enhanced
rm(list=ls())
setwd("P:/Evaluation/TN Lives Count_Writing/3_Target1_SUICClinicalTrainingComparison/3_Data & Analyses")
datPre = read.csv("Pre.csv", header = FALSE, row.names = NULL)
setwd("P:/Evaluation/TN Lives Count_Writing/3_Target1_SUICClinicalTrainingComparison/3_Data & Analyses")
datPost = read.csv("Post.csv", header = FALSE, row.names = NULL)

#RCS
rm(list=ls())
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/RCS/Data")
dat = read.csv("AAC_RCS_Intake_Clean.csv", header = TRUE)

#Zero Suicide Data
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/ZeroSuicide")
ITSTest = read.csv("ZSData.csv", header = TRUE)
