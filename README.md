# Code Copier (Copy your code!)

Ever wanted to simply copy the codes in your file to share them or get help? Me too bro, me too.
This python script allows you to copy all the code in your files to a copyable text file. 
This is useful for creating a backup of your code or for sharing it online with friends or with LLMs.

1. List all items (files & subdirectories) in the current directory.  
2. Prompt the user to select items required.  
3. Recursively read files and then export their contents into a single output file.  
4. Mark image files with the text `IMAGE` instead of dumping their binary data.  
5. Recursively handle subdir if theya re in the selection.
6. Avoid copying itself (*the python script*) and the final export file (`writtencode.txt`) back into the output.

---


## Requirements

- **Python**  
- **(`os` library)**

---

## Usage

1. **Download or copy this script** into your target directory.  
2. **Open the terminal or ues your IDE** in the same directory where the script is located.  
3. **Run the script** by pressing play in your IDE or by typing:

```bash
python codecopier.py
```

4. **Follow the on-screen prompts** to select the items (files or directories) you wish to export.

After selecting items, the script will generate a file named **`writtencode.txt`** in the same directory.

5. **Open `writtencode.txt`** then select all and copy.
6. **Paste the copied content** into your desired location.


---

## File/Directory Selection Examples

1. **All items**  
   - Input: `0`  
   - Outcome: All listed items are copied.

2. **Multiple single picks**  
   - Input: `1 3 5`  
   - Outcome: Items #1, #3, #5 are copied.

3. **Ranges**  
   - Input: `1to4`  
   - Outcome: Items #1, #2, #3, #4 are copied.

4. **Mixed**  
   - Input: `2to4 6`  
   - Outcome: Items #2, #3, #4, #6 are copied.

---

## Notes

1. The subdir files are indicated as such so it is clear to the person reading `writtencode.txt` the format to better help you in your code.
2. You can easily change the name of the output file `writtencode.txt` in the first few lines of the program.
3. This script is designed to work without any libraries needed. You may add additional libraries to automatically copy the code to your clipboard.
However, I decided against this as that would increase the complexity for newer users who may find this program helpful.
