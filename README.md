# mri_s-s_Tools
MRI Sequences sorting &amp; Segamentation masking Toolbox. musical-potato-potatoes~ Or fluffy-octo-sniffle?
And please Don't read in preview if you want to understand how this stuff work.
  demo_Dicom_Classifyer5.m: It's my teacher Guoxi Xie's idea and I implement it with Matlab... 
    No other libs are required. Sucessfully tested on Matlab 2016a & Matlab 2016b
    pre-condition: In the selected direcotry the Dicom files are placed in the second layer of files. 
      example: 
            (Folder) Disease Name   <--The directory of this folder is placed in variable [PathRoot]
             |--(Folder) PatientName_studyDate 
             |   |---(Folder) Series_Num1
             |   |    |--(file1) file_nameA.dcm
             |   |    |--(file2) file_nameB.dcm
             |   |  
             |   |---(Folder) Series_Num2
             |        |--(file1) file_nameC.dcm
             |        |--(file2) file_nameD.dcm
             |--(Folder) PatientName_studyDate <--The directory of this folder is placed in variable [PathRoot]
                |---(Folder) Series_Num1
                |    |--(file1) file_nameA.dcm
                |    |--(file2) file_nameB.dcm
                |
                |---(Folder) Series_Num2
                     |--(file1) file_nameC.dcm
                     |--(file2) file_nameD.dcm
    post-condition: This scrip copy files and sort it by its pantient_name, study_date, Series_Description.
    
