1. Upload Your Python Script (.py File):

Open a new Colab notebook or use an existing one.
Click the "Files" tab on the left sidebar.
Click the "Upload" button near the top right corner.
Select your .py file and upload it.
You'll see your file listed under "Files" in the left sidebar.
2. Mount Google Drive (Optional, but Recommended for Datasets):

If your dataset is stored in your Google Drive, mounting your Drive allows you to access it from Colab.
In a code cell, type the following and run it (press Ctrl + Enter):
Python
from google.colab import drive
drive.mount('/content/drive')
Use code with caution.
content_copy
Follow the on-screen instructions to grant Colab access to your Drive. This process might require entering an authorization code.
3. Upload Your Dataset:

Option A: Uploading from Local Machine (for small datasets):

Click the "Upload" button again in the "Files" tab.
Select your dataset file(s) and upload them.
Option B: Uploading from Google Drive (for larger datasets or private storage):

Navigate to the directory in your Drive where your dataset is located.
Right-click on the dataset file(s) and select "Copy path."
In a code cell, use the !cp command to copy the file(s) from Drive to Colab's working directory. Replace <path_in_drive> with the copied path:
Python
!cp <path_in_drive> /content/
Use code with caution.
content_copy
4. Run Your Python Script:

Make sure your Python script's working directory is set correctly. If you uploaded the script and dataset within Colab, you shouldn't need to modify the working directory.

In a new code cell, use the !python command followed by the name of your .py file:

Python
!python your_script.py
Use code with caution.
content_copy
Replace your_script.py with the actual filename.

This will execute your script, and any code that interacts with the dataset (loading, processing, etc.) will be run.
