### RESEARCH DATA MANAGEMENT
#### Commonly used file and folder manipulation commands
In this notebook, I gather my commonly used python bits for file and folder manipulation. If you work with many different samples, tools and programs and frequently find yourself adding, deleting, renaming or replacing large numbers of files and/or directories, you might find this notebook useful. There are undoubtedly better ways of doing some of these things so feel free to suggest improvements.

I generally like to keep the directory structure relatively flat to avoid lots of navigating. In my research, I use 5 - 6 different programs and tools that generate a few files each. I use the following directory structure:
```
project
│    dir_list.txt
│
└─── sample_1
│   │
│   └─── tool_1
│   │   │   tool_1_file_1
│   │   │   tool_1_file_2
│   │   │   ...
│   │
│   └─── tool_2
│   │   │   tool_2_file_1
│   │   │   tool_2_file_2
│   │   │   ...
│   │
│   └─── ...
│
└─── sample_2
│   └─── ...
│ ...
```
This helps to keep the data organized and allows easy access to the corresponding files and directories using the steps below. The file `dir_list.txt` contains the absolute paths to the directories `sample_1`, `sample_2`, etc. (see step 1) and serves as the entry-point for most operations. It also allows you to gather all the data in a single dataframe to perform analysis (see step 7).