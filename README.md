# open_Jupyter.bat
Use bat to open jupyter on anaconda and env and chamge disk

## Use .bat to open Jupyterlab
1.1 Make a copy for activate.bat 

  C:\Users\EOSPHD\anaconda3\Scripts\activate.bat 
  
  C:\Users\EOSPHD\anaconda3\Scripts\activate_julab.bat
 
1.2 Add 「 @CALL jupyter lab 」 at the bottom of the new bat

    @REM This may work if there are spaces in anything in %*
    @CALL "%~dp0..\condabin\conda.bat" activate %*
    @CALL jupyter lab
    :End
    @set _args1_first=
    @set _args1_last=
    
2.1 New a bat to open activate_julab.bat
rem Change Disk
E:   

rem Change Folder
CD E:\Asbestos_UN 

rem use cmd to openjupyter Lab and set env
%windir%\System32\cmd.exe "/K" C:\Users\EOSPHD\anaconda3\Scripts\activate_julab.bat tf_2.5_py_3.8 

