Since there is no `Scripts` folder, it indicates that `pip` might not have been installed correctly. Let's go through the steps to ensure `pip` is properly installed:

1. **Re-download and run the `get-pip.py` script**:
    - Open your web browser and download the `get-pip.py` script from [this link](https://bootstrap.pypa.io/get-pip.py).
    - Save the file to your Desktop.

2. **Run the `get-pip.py` script**:
    - Open a command prompt and navigate to the Desktop directory by running:
      ```sh
      cd Desktop
      ```
    - Run the script to install `pip`:
      ```sh
      python get-pip.py
      ```

3. **Check the installation directory**:
    - After running `get-pip.py`, check if a `Scripts` folder is created in the Python installation directory (`C:\Users\xxx\Desktop`). It should contain the `pip` executable.

4. **Add `pip` to the PATH environment variable**:
    - If the `Scripts` folder exists, add it to your PATH:
      - Open the System Properties:
          - Right-click on "This PC" or "Computer" on the desktop or in File Explorer.
          - Click "Properties."
          - Click "Advanced system settings."
          - Click "Environment Variables."
      - In the Environment Variables window, find the `Path` variable in the "System variables" section and select it.
      - Click "Edit."
      - In the Edit Environment Variable window, click "New" and add the path to the `Scripts` directory (`C:\Users\xxx\Desktop\Scripts`).
      - Click "OK" to close all windows.
      - Close the command prompt and open a new one to apply the changes.

5. **Verify the `pip` installation**:
    - Open a new command prompt and type:
      ```sh
      pip --version
      ```
    - It should display the version of `pip` installed, indicating that `pip` is now recognized.

6. **Install PyQt5**:
    - Once `pip` is recognized, you can install PyQt5 by running:
      ```sh
      pip install PyQt5
      ```

If the `Scripts` folder is still not created after running the `get-pip.py` script, please let me know so I can explore alternative methods to install `pip`.
