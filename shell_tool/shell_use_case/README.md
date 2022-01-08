



- List the 

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