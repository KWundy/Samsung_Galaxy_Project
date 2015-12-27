features <- read.table("~/UCI HAR Dataset/features.txt", quote="\"", comment.char="")
features[,2]->vars
dQuote(vars)->vars

X_test <- read.table("~/UCI HAR Dataset/test/X_test.txt",col.names = vars,quote="\"", comment.char="")
X_train <- read.table("~/UCI HAR Dataset/train/X_train.txt",col.names = vars ,quote="\"", comment.char="")
rbind(X_train,X_test)->X_bind

select(.data = X_bind,contains("std",ignore.case=TRUE))->X_sd
select(.data = X_bind,contains("mean",ignore.case=TRUE))->X_means
cbind(X_means,X_sd)->X_msd

as.data.frame(colSums(X_msd)/nrow(X_msd))->averages
names(averages)<-c("total_average")
