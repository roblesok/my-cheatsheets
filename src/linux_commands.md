# Linux Common Commands

## FIND

```
-- Find files recursively
find . -name '*.txt' -type f

-- Delete files recursively
find . -name '*.txt' -type f -delete

-- Find directories recursively
find . -name 'node_modules' -type d

-- Delete directories recursively
find . -name 'node_modules' -type d print0 | xargs -0 rm -rf
```

## GREP

```
-- matching word (ignore-case)
grep -i "hello"

-- match lines that start with some word
grep "^hello" filename

-- match lines that end with word
grep "finish.$" filename
```

## CURL

```
-- downland and display progress
curl -# -o myfile.zip ftp://...file.zip

-- downland and maintain original name
curl -# -O ftp://...file.zip

-- Download with auth 
curl -u username:password -O ftp://...file.zip

-- Upload file 
curl -u username:passwrod -T {fname} {ftp_location}
```

