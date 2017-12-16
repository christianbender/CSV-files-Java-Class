## CSVFile class

This class contains a data structure and some useful methods 
to deal with CSV files under JAVA. The class contains three different
constructors (see below).

### Overview

* CSVFile(path : string, seperator : char)

    compiles the CSV-file in the inner data structure.

    * CSVFile (file : File, seperator : char)


    * CSVFile (seperator : char)

        for empty CSV-file

* compile (row : string, seperator : char) : string

    compiles row in its columns.

* isPunctuation (ch : char) : boolean
 
    check whether ch is a punctuation character.

* getElementString(row : int, column : int) : string
 
 	returns the specified element.
 
 * getElementDouble(row : int, column : int) : double
 
    returns the specified element as double.
 
* addRow(row : string) : void
 
    adds a row to the inner data structure. without writing into the CSV-file.

* set (row : int, column : int, item : string) : void
 
    replaces the specified item with a newer.
 
* commit() : void 
 
    writes the added data into CSV-file.
  
    * commit(path : String) : void
    * commit(file : File ) : void
 
* findRow(key : string) : ArrayList<String>
 
  	returns the searched row otherwise null.

* contains(key : string) : boolean
 
    returns true if a row contains 'key' otherwise false.
  
* getColumn(column : int) : ArrayList<String>
 
    returns the specified column as ArrayList.
  
    * getColumn(key : string) : ArrayList<String>
 
* removeRow(key : string) : void 
 
 	purpose removes the specified row at the inner data structure.
  
    * removeRow(column : int) : void

* updateFile() : void
 
    overwrites the CSV-file with the current inner data structure.
    
    removed rows are remove in the CSV-file, too.
 
    * updateFile(file : File) : void
  
* getNumberOfRows() : int

 returns the number of rows in CSV-File
 
 it counts only rows that in the table.
