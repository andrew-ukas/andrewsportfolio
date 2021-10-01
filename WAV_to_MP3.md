# How to convert a WAV file to an MP3 file with FFmpeg in Windows Powershell 
### Written by Andrew Saku
Audio files come in different forms, such as WAV or MP3. Certain programs only utilize certain file types, so it's useful to know how to convert between file types easily. In this example, you will learn how to convert a WAV file to an MP3. You can use these same principles to convert media files to other media types, such as converting audio to other audio file types (.ogg, .m4a) or converting audio to video (.mp4, .mov, .mkv) and vice versa. 

1. Ensure you have FFmpeg installed. If not, refer to instructions [here](https://www.wikihow.com/Install-FFmpeg-on-Windows) for installation. 
2. Go to the folder in which you have the file you want to convert.
3. Highlight all text in the address bar. Type `powershell`. Press *Enter* on your keyboard. This will open a Windows Powershell command line. 
4. In the command line, type `Get-Childitem`. This will display all the file names in the folder. Find the name of the WAV file you would like to convert. We will refer to the desired file as `input.wav`.
5. Choose a file name for the desired output MP3 file. We will refer to the output file as `output.wav`. 
6. In the command line, type 

        ffmpeg -i input.wav output.mp3 
    Press *Enter*. 

7. You will now have an MP3 copy of the WAV file you previously had. Type and enter “Get-Childitem” in the powershell window to confirm, or go to the File Explorer window.

Things to keep in mind:
	If your file name has spaces in it, you will want to put quotation marks around the file. 
		Example: Use the file name "your_file_name.wav" as opposed to “your file name.wav”
