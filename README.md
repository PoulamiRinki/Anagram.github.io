<!DOCTYPE html>
<html lang="en">
    <head>
         <meta charset="UTF-8"> 
         <meta http-equiv="X-UA-Compatable" content="IE=edge"> 
         <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
         <title> Anagram</title> 
         <link rel="stylesheet" href="index.css" />
        </head>
        <body> 
            <div class="square"> </div>
    <script>

    // JavaScript program to check whether two strings
    // are anagrams of each other
    
        /* function to check whether two strings are
        anagram of each other */
        function areAnagram(str1,str2)
        {
            // Get lenghts of both strings
            let n1 = str1.length;
            let n2 = str2.length;
    
            // If length of both strings is not same,
            // then they cannot be anagram
            if (n1 != n2)
                return false;
    
            // Sort both strings
            str1.sort();
            str2.sort()
    
            // Compare sorted strings
            for (let i = 0; i < n1; i++)
                if (str1[i] != str2[i])
                    return false;
    
            return true;
        }
        
        /* Driver Code*/
        let str1= window.prompt("Enter first string:");
        
        let str2= window.prompt("Enter Second string:");
        
        
        // Function Call
            if (areAnagram(str1, str2))
                document.write("The two strings are"
                                + " anagram of each other<br>");
            else
                document.write("The two strings are not"
                                + " anagram of each other<br>");
    
    
    
    
    
    // This code is contributed by rag2127
    
    </script>
    </body>
</html>
    
