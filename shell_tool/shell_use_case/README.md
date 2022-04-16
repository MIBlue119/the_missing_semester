



- List the files/ directoris numbers 
```
$ls | wc -l 
```

- Export the datetime/uptime/uname info result to a txt file
```
$(date; uptime; uname -r) > myfile.txt 
```

- Grep a specific info at the file's content
```
$cat myfile.txt | grep the_patterns_you_want
```
    - `|` is a pipe command. 
        - It could let the previous command's output as the next command's input
- Find the specific file types and grep the filename with specific patterns
```
$find . -name "*.py" | grep "mdx" 
```
    - It may return like this
    ```
    ./demucs/grids/mdx_refine.py
    ./demucs/grids/mdx.py
    ./demucs/grids/mdx_extra.py
    ```
            
- Show the all files under the director and sort them in human-readable sizes
```
$du -h | sort -h 
```
    - Show the files with specific size
    ```
    $du -sh * | sort -n | grep G
    ```
- Show the current directory mounted space in human readable format
```
$df -h . 
```

- Show the port used by which PID(Process Identification)
    - Example: grep the 3000 port 
    ```
    $sudo nestat -lpn| grep 3000
    ```
        - If you want to terminate the PID
        ```
        $kill <number_of_PID>
        ```