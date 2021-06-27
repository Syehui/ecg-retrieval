# ecg-retrieval

数据集：
	1.下载和准备所有数据集：ecg-retrieval\data\prepare-every-dataset
	
		physione数据源：
		https://raw.githubusercontent.com/physionetchallenges/physionetchallenges.github.io/master/2020/Dx_map.csv
		https://cloudypipeline.com:9555/api/download/physionet2020training/PhysioNetChallenge2020_Training_CPSC.tar.gz/
		https://cloudypipeline.com:9555/api/download/physionet2020training/PhysioNetChallenge2020_Training_PTB.tar.gz/
		https://cloudypipeline.com:9555/api/download/physionet2020training/PhysioNetChallenge2020_Training_E.tar.gz/
		https://cloudypipeline.com:9555/api/download/physionet2020training/PhysioNetChallenge2020_Training_StPetersburg.tar.gz/
		https://cloudypipeline.com:9555/api/download/physionet2020training/PhysioNetChallenge2020_Training_2.tar.gz/
		https://cloudypipeline.com:9555/api/download/physionet2020training/PhysioNetChallenge2020_PTB-XL.tar.gz/

		edar数据集数据源：
		https://s3-eu-west-1.amazonaws.com/pfigshare-u-files/15651296/RhythmNames.xlsx
		https://s3-eu-west-1.amazonaws.com/pfigshare-u-files/15652862/ECGDataDenoised.zip
		https://s3-eu-west-1.amazonaws.com/pfigshare-u-files/15653123/AttributesDictionary.xlsx
		https://s3-eu-west-1.amazonaws.com/pfigshare-u-files/15651299/Diagnostics.xlsx
		https://s3-eu-west-1.amazonaws.com/pfigshare-u-files/15651293/ConditionNames.xlsx
		https://s3-eu-west-1.amazonaws.com/pfigshare-u-files/15651326/ECGData.zip

		天池数据集：
		http://tianchi-competition.oss-cn-hangzhou.aliyuncs.com/231754/round2/hf_round2_train.zip
		http://tianchi-competition.oss-cn-hangzhou.aliyuncs.com/231754/round2/hf_round2_train.txt
		http://tianchi-competition.oss-cn-hangzhou.aliyuncs.com/231754/round2/hf_round2_arrythmia.txt
	2.合并数据集：ecg-retrieval\data\prepare-final-data
	3.得到"相似患者检索实验"训练数据集：ecg-retrieval\data\get-final-data
	4.得到"同身份患者检索实验"训练数据集：ecg-retrieval\data\get-ecg-recognition-data.ipynb
	5.ecg去噪：ecg-retrieval\data\ecg-data-denosing.ipynb
训练和评估：

	相似患者检索实验：ecg-retrieval\trainjob\ecg-retrieval-similar-trainjob.ipynb
	同身份患者检索实验：ecg-retrieval\trainjob\ecg-retrieval-regconition-trainjob.ipynb
