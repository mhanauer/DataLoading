setwd("~/Desktop")
write.csv(data.frameNames, "data.frameNames.csv", row.names = FALSE)
data.frameNames = read.csv("data.frameNames.csv", header = TRUE, na.strings = c("na", " "))
data.frameNames


## Gatekeeper
rm(list=ls())
setwd("P:/Evaluation/TN Lives Count_Writing/3_Target1_SUICClinicalTrainingComparison/3_Data & Analyses")
datPre = read.csv("Pre.csv", header = FALSE, row.names = NULL)
datPost = read.csv("Post.csv", header = FALSE, row.names = NULL)
dat3month = read.csv("3month.csv", header  = TRUE)

#Connections
rm(list=ls())
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/ConnectionsPaperData")
GPRAAll = read.csv("ConnGPRA.csv", header = TRUE, na.strings = c(-9, -8, -7, -1, "", " ", "NULL", NULL, NA, "NA")) 
PHQ9Base = read.spss("S:/Indiana Research & Evaluation/Indiana Connections/Data/PHQ9/PHQ9 Baseline.sav", to.data.frame = TRUE)
GAD7Base = read.spss("S:/Indiana Research & Evaluation/Indiana Connections/Data/GAD7/GAD7 Baseline.sav", to.data.frame = TRUE)
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

## Adult Health Home Outcomes
rm(list=ls())
setwd("T:/Clinical Model Materials/Clinical Models/Adult Health Home/Evaluation Materials/Data/2. Vitals/3. October 2018/Matt'sData")
CIL_South_HCS_vitals_10052018 = read.csv("CIL_South_HCS_vitals_10052018.csv", header = TRUE)
CIL_west_HCS_vitals_10052018 = read.csv("CIL_west_HCS_vitals_10052018.csv", header = TRUE)
CIN_HCS_Vitals_10052018 = read.csv("CIN_HCS_Vitals_10052018.csv", header = TRUE)
CKY_HCS_Vitals_10052018 = read.csv("CKY_HCS_Vitals_10052018.csv", header = TRUE)

setwd("T:/Clinical Model Materials/Clinical Models/Adult Health Home/Evaluation Materials/Data/10. PHQ9/October 2018/Matt'sData")
CIL_South_HCS_PHQ9_10102018 = read.csv("CIL_South_HCS_PHQ9_10102018.csv", header= TRUE)
CIL_West_HCS_PHQ9_10102018 = read.csv("CIL_West_HCS_PHQ9_10102018.csv", header= TRUE)
CIN_HCS_PHQ9_10102018 = read.csv("CIN_HCS_PHQ9_10102018.csv", header = TRUE)
CKY_HCS_PHQ9_10102018 = read.csv("CKY_HCS_PHQ9_10102018.csv", header = TRUE)

setwd("T:/Clinical Model Materials/Clinical Models/Adult Health Home/Evaluation Materials/Data/11. Tobacco/October 2018/Matt'sData")
CIL_South_HCS_Tobacco_10052018 = read.csv("CIL_South_HCS_Tobacco_10052018.csv", header = TRUE)
CIL_west_HCS_Tobacco_10052018 = read.csv("CIL_west_HCS_Tobacco_10052018.csv", header = TRUE)
CIN_HCS_Tobacco_10052018 = read.csv("CIN_HCS_Tobacco_10052018.csv", header = TRUE)
CKY_HCS_Tobacco_10052018 = read.csv("CKY_HCS_Tobacco_10052018.csv", header= TRUE)


setwd("T:/Clinical Model Materials/Clinical Models/Adult Health Home/Evaluation Materials/Data/7. Enrollment Lists/November 2018/Matt'sData")
HCS_Enrollment_Demo = read.csv("HCS_Enrollment_Demo.csv", header= TRUE)

#Enhanced
rm(list=ls())
setwd("P:/Evaluation/TN Lives Count_Writing/4_Target1_EnhancedCrisisFollow-up/3_Data & Data Analyses")
datPreAdult = read.csv("Target1EnhancedBaseAdult.csv", header = TRUE)
datPostAdult = read.csv("Target1EnhancedPostAdult.csv", header = TRUE)
datAdultTreat = read.csv("AdultTreatments.csv", header = TRUE)
#describe.factor(datAdultTreat$Treatment)

###CCPE Numbers
setwd("C:/Users/Matthew.Hanauer/Desktop")
ccpe_numbers = read.csv("CCPENumbers.csv", header = TRUE)


#install.packages("countreg", repos=http://R-Forge.R-project.org)

#RCS
rm(list=ls())
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/RCS/Data")
dat = read.csv("AAC_RCS_Intake_Clean.csv", header = TRUE)

#Zero Suicide Data
rm(list=ls())
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/ZeroSuicide")
ITSTest = read.csv("ZSData.csv", header = TRUE, na.strings = "N/A")
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/ZeroSuicide")
ITSRolling = read.csv("ZeroSuicideRollingSum.csv", header = TRUE, na.strings = "N/A")
InSuicides = read.csv("INSuicides.csv", header = TRUE)
TotalCount = read.csv("TotalCount.csv", header = TRUE)
#### Rate Zero Suicide
setwd("P:/Evaluation/TN Lives Count_Writing/ZeroSuicide/Matt'sData")
zero_suicide = read.csv("zero_suicide.csv", header= TRUE, na.strings = c("multiple ???", "NA"))
zero_suicide_denom = read.csv("zero_suicide_denom.csv", header = TRUE)

#Enhanced Bayes
setwd("P:/Evaluation/TN Lives Count_Writing/4_Target1_EnhancedCrisisFollow-up/3_Data & Data Analyses")
dat = read.csv("EnhancedDataSet.csv", header = TRUE)
#setwd("C:/Users/Matthew.Hanauer/Desktop/BEST")
#source("BEST.R")


#FISCH Data
setwd("S:/Indiana Research & Evaluation/FISCH (Jon's Study)/Data")
data_FISCH = read.csv("FISCH_DATA_2019-06-11_1120.csv", header = TRUE)
enrollment = read.csv("EnrollmentDate6_11_2019.csv", header = TRUE)
### CCPE Youth data
setwd("S:/Indiana Research & Evaluation/CCPE/CCPE SPSS - Datasets/YOUTH Datasets")
BaseYouth = read.csv("Baseline CCPE GPRA Youth.csv", header= TRUE, na.strings = c(97,98,99))
ReassessYouth = read.csv("Reassess 3M CCPE GPRA Youth.csv", header = TRUE, na.strings = c(97,98,99))

### FHHC
setwd("S:/Indiana Research & Evaluation/FHHC Homelessness/Data and QPR")
base = read.csv("FHHC_Base.csv", header = TRUE, na.strings = c())
FHHC_redcap= read.csv("FHHC_redcap.csv", header = TRUE, na.strings = c(-4,-99, -97, -98, -99,-1))
FHHC = read.csv("FHHC.csv", header = TRUE, na.strings = c(-4,-99, -97, -98, -99,-1))


#### CCPE Data set
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/CCPEPaperData")
CCPEBaseline = read.csv("CCPEBaselineFull.csv", header = TRUE)

### Concept mapping testing
setwd("C:/Users/Matthew.Hanauer/Desktop")
datTest = read.csv("datCorMD.csv", header = TRUE)

#### Enhanced Auto content
setwd("P:/Evaluation/TN Lives Count_Writing/4_Target1_EnhancedCrisisFollow-up/3_Data & Data Analyses")
adult = read.csv("Target1EnhancedPostAdult.csv", header = TRUE, na.strings = c(-99, 9, -9, "", NA, "N/A", "NA", -8, " "))
youth = read.csv("TargetYouth_clean.csv", header = TRUE, na.strings = c(-99, 9, -9, "", NA, "N/A", -8, "NA", -8," "))
setwd("P:/Evaluation/TN Lives Count_Writing/4_Target1_EnhancedCrisisFollow-up/3_Data & Data Analyses/AutoContent")

###AMA 
rm(list=ls())
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/AMAData")
AMAData = read.csv("AMAData.csv", header = TRUE, na.strings = c("NULL", "N/A"))

setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/AMAData")
edu_dat = read.csv("Education.csv", header = TRUE)

### SASSI
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/SASSI/Data")
honest = read.csv("A3 Honest Admin.csv", header = TRUE)
fake = read.csv("A3 Fake-Good Admin.csv", header = TRUE)

####CCPE New GPRA
setwd("S:/Indiana Research & Evaluation/CCPE/NewGPRAData")
base = read.csv("baseline.csv", header = TRUE, na.strings = c(-99, -98, -97))
month6 = read.csv("month6.csv", header = TRUE, na.strings = c(-99, -98, -97))

###CCBHC
setwd("P:/Evaluation/CCBHC IN/Data")
ccbhc_adult = read.csv("Adult data.csv", header = TRUE, na.strings = c(-1:-11))
setwd("P:/Evaluation/CCBHC IN/Data")
ccbhc_child = read.csv("Youth data.csv", header = TRUE, na.strings = c(-1:-11))

###EMERGE
setwd("S:/Indiana Research & Evaluation/EMERGE CRR/Data")
base = read.csv("base.csv", header = TRUE)
month6 = read.csv("month6.csv", header = TRUE)


##FHHC reports
setwd("S:/Indiana Research & Evaluation/FHHC Homelessness/Data and QPR")
base = read.csv("FHHC_base.csv", header = TRUE, na.strings = c(-99, -98, -97, " "))
month6 = read.csv("FHHC_Month6.csv", header = TRUE, na.string = c(-99, -98, -97, " "))
FHHC = read.csv("FHHC.csv", header = TRUE, na.string = c(-99, -98, -97, -1, -4, -5, -7, -9, -2, -6 -8, " "))
dim(month6)
dim(base)

## Zero Indiv
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/ZeroSuicide")
indiv_dat = read.csv("AO Log  consolidated 2002-2019.csv", header = TRUE, na.strings = c("unknown", "?", "", " ", "???","```", "??","10-Apr"))
## Revenue data
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/SustainWorkshop/RevenueAnalysis")
CIN_revenue = read.csv("CH17-37_20190731_123328.csv", header = TRUE)
##HRSA
setwd("S:/Indiana Research & Evaluation/HRSA Healthy Start/Monthly Client-Level Data - HSMED/July 2019")
hrsa = read.csv("July 2019 Data Export.csv", header = TRUE)
##CCPE Ad Hoc report
setwd("S:/Indiana Research & Evaluation/CCPE/Reports/AdHocReport")
CCPE_report = read.csv("gpraAdultAll.csv", header = TRUE, na.strings = c(-99, 98, 97))
### TLC Connect 2019
setwd("P:/Evaluation/TN Lives Count_Connect/Databases")
tlc_data = read.csv("TLCConnect_10_1_2019.csv", header = TRUE, na.strings = c(-6,-7,-8,-9))

### Cluster AEA 2019
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/AEA2019")
cluster_data = read.csv("Demographics by location.csv", header = TRUE)

#### CCPE SPARS report upload
setwd("S:/Indiana Research & Evaluation/CCPE/NewGPRAData")
base = read.csv("Year4data_baseline.csv", header = TRUE, na.strings = c(-99, -98, -97))

setwd("S:/Indiana Research & Evaluation/CCPE/NewGPRAData")
base = read.csv("baseline.csv", header = TRUE, na.strings = c(-99, -98, -97))

##revenue
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/SustainWorkshop/RevenueAnalysis")
CIN_revenue = read.csv("CH17-37_20190731_123328.csv", header = TRUE)

# Centerstone study 2019-2020
setwd("S:/Indiana Research & Evaluation/Matthew Hanauer/Centerstone_Study_2019_2020")
center_dat = read.csv("BelongGive_DataClean_7.20.csv", header = TRUE)
