- 👋 Hi, I’m @Igluminati
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Igluminati/Igluminati is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

| Browser | Browser Stat Counter March 2021 | Net Market Share March 2021 | Wikimedia November 2019 |
| ------- | :-----------------------------: | :-------------------------: | :---------------------: |
| Chrome  | 64.91%                          | 66.43%                      | 48.7%                   |
| Safari  | 19.03%                          | 12.74%                      | 22.0%                   |
| Edge    | 3.74%                           | 5.07%                       | 1.9%                    |
| Firefox | 3.68%                           | 3.62%                       | 4.9%                    |
| Samsung Internet | 3.27%                  | 3.29%                       | 2.7%                    | 
| Opera   | 2.13%                           | 1.51%                       | 1.1%                    |
| IE      | 0.73%                           | 1.76%                       | 3.9%                    |
| Others  | 3.23%                           | 5.58%                       | 14.5%                   |

# Unix Mission

### Finding the diamonds

To find the diamonds, I used the following command:
```
grep -Rw ~/cs1998-mission/ -e 'diamond'
```
Where the ``-R`` option tells **grep** to read all files under each directory recursively, and the ``-w`` option instructs it to only select lines containing matches. The ``-e`` option is used to specify the string to be searched, in this case **'diamond'**.

This allowed me to discover that the diamonds were located in the following paths:
```
/home/cim/ug/zjac300/cs1998-mission/south/west/north/bag:a pink diamond
/home/cim/ug/zjac300/cs1998-mission/north/west/west/bag:a precious diamond
/home/cim/ug/zjac300/cs1998-mission/west/west/east/bag:a blue diamond
```

### Deleting all the bags that do not contain diamonds
To do this task, I used a command to find all files which did **not** include the 'diamond' string 
```
grep -Rw ~/cs1998-mission/ -Z -L -e 'diamond' | xargs --null rm
```
The ``-Z`` argument allows for the command to print with a null terminator rather than the usual newline seperator, whereas the ``-L`` argument allows grep to print the filenames of those files on its command line which **do not** match the regular expression **'diamond'**. Lastly, the ``--null`` argument tells xargs to accept null-terminated inputs which in turn allows the ``rm`` to remove said input (in this case the filenames of those files without the **'diamond'** string).

### Deleting the directories on the paths that do not lead to diamonds
As all the directories on the paths that do not lead to diamonds are now empty, I used the command to delete all empty directories:
```
find . -empty -type d -delete
```
Where the ``-empty -type d`` option implies that the command only applies to **empty directories**, and ``-delete`` indicating that the ``find`` command should delete all **empty directories** 

### My completion code: ``zjac300-395a291536``
