
# Ruleset

TODO add links to for each justification
TODO separate out sections with headers

  - package level
    - declaration
      - type (struct/interfaces) 
        - comments on line width may extend to 140 characters                                                                                                           
      - var/const
        - merge 2 or more subsiquent delarations into a group declaration
      - functions 
        - minimum wrap size 50
        - maximum wrap size 120 
        - wrap functions at the nearest breakpoint closest to the maximum 
          line number 
        - newline for function outputs should only begin after the `) (` 
        - Header comment
          - All general comments rules apply ----------------- TODO LINK
          - Usage of `NOTE`
            - all `NOTE`s should be located at the end of the header comment
            - if multiple lines are used for the explanation following the 
              `NOTE` then entire contents of the note lines should be word 
              wrapped and begin at the 
              first character 
          - Usage of bullet points. 
            - if bullet points exist within the function header comment
      - section breaks
        - line section breaks should be composed of underscores (`_`)
          - the length of section breaks should not >= the maximum line 
            length of the surrounding +- 40 lines
          - exception: maximum value of 120 characters 
  - function level (aka within a function) 
      - var/const
        - never use group declaration
  - structs 
    - object declaration
      - do not allow one line struct object declaration which utilize field names in declartion                                                   
  - general comments
    - word wrap length 
      - apply 
    - paragraph comments extending beyond 3 lines should be word wrapped 
    - paragraph comments extending below 2 lines should be separated by sentence
      - unless a sentence must be word wrapped in which case the entire paragraph should
        be word wrapped 
    - Usage of bullet points. 
      - if bullet points exist within the function header comment
    -  

## Rule of variable wrapping 

There are different appropriate lengths for which:
 - comments, 
 - function headers, and 
 - function contents

should be wrapped at. In general the principal applied is to balance between:
 - keeping lines within the functions capped at a similar length
 - keeping the line length long enough to allow for compact code with good
   visual queues 

Determining the variable wrap length
 - Within a function:
   - > 10 lines of code exist _within_ function the 90th percentile 
     maximum line length should be used.
   - <= 10 lines exist - wrap any line which is greater than 100
     characters. 

