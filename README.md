# Arrays
 
  Arrays are useful tools that allow us to store multiple varaibles of the same type. Each array
 begins at 0 and will increase to up to one less than its length (because we start at 0, not 1)
 An array of length 10 will have index values of 0 - 9, an example below
 
     ["Test1", "Test2", "Test3", "Test4", "Test5", "Test6", "Test7", "Test8", "Test9", "Test10"]
      0           1         2       3        4         5       6        7        8        9
 
 to delcare an array, we can use the following syntax
 
        var arrayName : [type] = []
 
 This will create an empty array of the specified type. Swift has type inference of arrays, but it is good
 practice to specify the type so you can quickly see what the array is storing quickly
 
 Here are examples of below empty arrays of each primitive type, empty and filled
 
     var arrayOfInts : [Int] = [ ]
     var arrayOfStrings : [String] = [ ]
     var arrayOfDoubles : [Double] = [ ]
     var arrayOfBools : [Bool] = [ ]
     
     var arrayOfInts : [Int] = [1, 2, 3, 4, 5]
     var arrayOfStrings : [String] = ["One", "Two", "Three", "Four", "Five"]
     var arrayOfDoubles : [Double] = [1.0, 2.0, 3.0, 4.0, 5.0]
     var arrayOfBools : [Bool] = [true, false, true, false, true]

 There are also tools that we can use to modify arrays very easily, these methods are
 
        - append : Add an item onto the end of an array
            Usage:
                 var arrayOfInts : [Int] = [1, 2, 3, 4, 5]
                 print(arrayOfInts)
                 arrayOfInts.append(6)
                 print(arrayOfInts)
            Output:
                 [1, 2, 3, 4, 5]
                 [1, 2, 3, 4, 5, 6]
 
        - + : you can use the plus operator to add contents of two arrays together (it will append the second array to the end of the first array
            Usage:
                var array1 : [String] = ["Practice"]
                print(array1)
                var array2 : [String] = ["Test"]
                print(array2)
                var array3 : [String] = array1 + array2
                print(array3)
 
            Output:
                ["Practice"]
                ["Test"]
                ["Practice", "Test"]
 
        - insert : insert allows you to place a specific item into your array at the specified index
     
            Usage:
                 var array4 : [String] = ["Practice" , "Test"]
                 print(array4)
                 array4.insert("A" , at: 1)
                 print(array4)
            Output:
                 ["Practice", "Test"]
                 ["Practice", "A", "Test"]
 
        -removeAll : deletes the contents of the array used to call to call the method
     
            Usage:
                 var array4 : [String] = ["Practice" , "Test"]
                 print(array4)
                 array4.removeAll()
                 print(array4)
            Output:
                 ["Practice", "Test"]
                 []
    
There are lots of ways to manipulate arrays using methods and index calling, the more practice you do with them to more methods you will discover!
    More practice: https://www.programiz.com/swift-programming/arrays
