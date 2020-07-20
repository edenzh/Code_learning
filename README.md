## Intruduction
My first repository for C++ and Python language learning and also some computer coding program useful information.

## Reference:
1. <Starting out with C++ from control structures through Objects> sixth edition. Tony Gaddis.
2. <Introduction to programming with C++> Y.Daniel Liang
3. <Starting out with Python> second edition, Tony Gaddis

## Enter to C++

## Enter to Python

## some useful information
### 1. vi command 
* Cursor movement—h, j, k, l (left, down, up, and right)
* Delete character—x
* Delete line—dd
* Mode toggle — Esc, Insert (or i)
* Quit—:q
* Quit without saving — :q!
* Run a shell command — :sh (use 'exit' to return)
* Save file — :w
* Text search — /
* formatting gg=G

---------------------------------------
THREE STATES 
---------------------------------------
STATE						           How to Get There

Command mode (where keys perform commands)  		    Hit 
Insert mode (where you can type information)		    Hit 'i' or 'a'
ed command-line mode (enter ed commands after the :)        Hit  : 

-----------------------
STARTING vi
-----------------------

    vi            | Edit a new or existing file

-----------------------
MOVING THE CURSOR
-----------------------

the following commands require that you hit  to enter 
command mode (unless you are already there...)
Commands prefaced by :  assume you are in command-line mode.

      h 		left.
      l 		right.
      k 		up.
      j 		down.
      $ 		end of line.
      ^ 		beginning of line.
      G 		end of document. 
      G    		To the nth line from top of document.
     :		To the nth line from the top of the document.
      /  	To .

-------------------
UNDOING CHANGES 
------------------
    u                       | Undo the latest change.
    U                       | Undo all changes on a line, while not having
                            |   moved off it (unfortunately).
    :q!                     | Quit vi without writing.
    :e!                     | Re-edit a messed-up file.

--------------------
ENTERING TEXT  
------------------- 

      a                  | append 
      i                  | insert

------------------- 
MISCELLANEOUS 
------------------- 
      J			| join current line with next line
      /fubar            | find next occurance of 'fubar'
      n                 | repeat last command one time  
      CTRL-g            | display current line number
      ^L                | Refresh the screen (sometimes `^P' or `^R').
      :set showmode     | will display INPUT MODE    

------------------- 
DELETING TEXT
------------------- 

      x                  Delete <*> chars under and after the cursor.
      X               <*> chars before the cursor.
      dd               lines.
      D                  delete the rest of the line.
      p			 will paste the deleted text into current line


------------------- 
SAVING WORK AND EXITING 
------------------- 

    :q                      | Quit vi, unless the buffer has been changed.
    :q!                     | Quit vi without writing.
    ^Z                      | Suspend vi.
    :w                      | Write the file.
    :w                | Write to the file .
    :w >>             | Append the buffer to the file .
    :w!               | Overwrite the file .
    :x,y w            | Write lines x through y to the file .
    :wq                     | Write the file and quit vi; some versions quit
                            |   even if the write was unsuccessful!
                            |   Use `ZZ' instead.
    ZZ                      | Write if the buffer has been changed, and
                            |   quit vi.  If you have invoked vi with the `-r'
                            |   option, you'd better write the file
                            |   explicitly (`w' or `w!'), or quit the
                            |   editor explicitly (`q!') if you don't want
                            |   to overwrite the file - some versions of vi
    :e                | Edit another file without quitting vi - the
                              text can be copied from one file to
                            |   another this way.

-----------------------
SHELL COMMANDS
-----------------------
    :sh                     | Execute a subshell, back to vi by `^D'.
    :r                | Read the file  into the buffer.
