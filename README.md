# Facial-Recognition-with-Machine-Learning

Edited From: RAHUL RANJAN, Avi Nehemiah, MATHWORKS & MATLAB Applications<br>
<br>
Authors: Timothy F. (CSC 6630/tfisher10), Kevin S.(CSC 4630/kseveur1), Micheal M.<br>
(CSC 4630/ mmoloney1), Adrian M.(CSC 4630/amcghee3)<br>
<br>
<br>
Description: To develop a GUI that recgonizes a face and matches it to the<br>
images GUI's database. The database will automatically check if the<br>
matched faced from the live captured image is present in the database.<br>
 <br>
Assumptions: <br>
- User knows basic usage of a computers components (mouse, keyboard,
webcam, etc.)<br>
- Must download the complete zip file and not edit the orgnization of the folders. <br>
- User has MATLAB2018a with Computer Vision toolbox, Image Acquistion<br>
toolbox,  Statitics and Machine Learning Toolbox and the <br>
correct video adapter for MATLAB installed. <br>
<br>
Usage:<br>
1.) In MATLAB Command Window, type TestVerification to begin the program. <br>
2.) First select the student's name you are trying to verify. This will begin the training and set the matching to the student's folder. ( Go to step 5 if student name is not in drop down box.)<br>
3.) Click the Verify ID then click Camera. Follow all the prompts in the message boxes and dialoge boxes.<br>
4.) If matched, then in the right window you will have a matched image from the database. If not matched then you will have a red x. <br>
5.) If student is not in the database then go to Database menu option. Then click New Student to add a new folder to FaceDatabaseFolder.<br> 
6.) Then add new student image by scrolling to Database then clicking New Student Picture to add a new student picture. Follow all the prompts.  <br>
7.) Reset the prgram after you added the new pictures. <br>
8.) Redo steps 1 through 4. <br>
9.) Quit the program when you are done.  <br>
<br>
Program Outline & Responsiblities (R)<br>
<br>
TestVerification.m<br>
    ...1.) R - Timothy F. / Adrian M.<br>
        ......GUI Initialization code (lines 31 to 48)<br>
        ......function TestVerification_OpeningFcn(hObject, eventdata, handles, varargin)<br>
        ......function varargout = TestVerification_OutputFcn(hObject, eventdata, handles)<br>
    <br>
    2.) R - Micheal M. <br>
<br>
        ...function Verify_Callback(hObject, eventdata, handles) <br>
        ...function Camera_Callback(hObject, eventdata, handles)<br>
<br>
    3.) R - Adrian M. / Timothy F. (RAHUL)<br>
<br>
        ...function Database_Callback(hObject, eventdata, handles)<br>
        ...function View_Callback(hObject, eventdata, handles)<br>
        ...function Picture_Callback(hObject, eventdata, handles)<br>
        ...function New_Student_Callback(hObject, eventdata, handles)<br>
<br>
    4.) R - Timothy F. <br>
<br>
        ...function Other_Callback(hObject, eventdata, handles)<br>
        ...function HE_LP_Callback(hObject, eventdata, handles)<br>
        <br>
        ...function Reset_Callback(hObject, eventdata, handles)<br>
        ...function All_Callback(hObject, eventdata, handles)<br>
<br>
        ...function Exit_Callback(hObject, eventdata, handles)<br>
        ...function Quit_Callback(hObject, eventdata, handles)<br>
<br>
    5.) R - Micheal M. <br>
<br>
        ...function Student_Select_Callback(hObject, eventdata, handles)<br>
<br>
        ...function Student_Select_CreateFcn(hObject, eventdata, handles)<br>
<br>
<br>
train_match.m (AVI)<br>
    1.) R - Micheal M. / Kevin S.<br>
        classdef train_match<br>
            properties<br>
            methods<br>
                function setStudentChoice<br>
                function train<br>
                function match<br>

Other Responsiblities:<br>
    ...Troubleshooting / Debugging: All<br>
    ...Ideas : All<br>
    ...Video Editing: Micheal M. <br>
<br>
<br>
Notes: <br>
- If you have a windows or linux system then use need to change the .m files code<br>
  to your respective adaptors.<br>
- Change the / to \ when using windows!!!!<br>
- Must install all the toolboxs/adaptors for this to fully function. <br>
- Keep the folder/file names consistent and keep the same structure as downloaded orginally.  <br>
<br>
