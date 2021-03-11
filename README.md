# Huffman-Coding
Python Implementation of Huffman Coding - compression and decompression

![x](https://user-images.githubusercontent.com/71879662/110761449-c1d9e800-8275-11eb-9197-07bd493ade9d.png)

Huffman Coding is one of the lossless data compression techniques. It assigns variable-length codes to the input characters, based on the frequencies of their occurence. The most frequent character is given the smallest length code.

## Data compression 

1.Building frequency dictionary<br/>
2.Select 2 minimum frequency symbols and merge them repeatedly: Used Min Heap<br/>
3.Build a tree of the above process: Created a HeapNode class and used objects to maintain tree structure<br/>
4.Assign code to characters: Recursively traversed the tree and assigned the corresponding codes<br/>
5.Encode the input text. Added padding to the encoded text, if it’s not of a length of multiple of 8. Stored this padding information, in 8 bits, in the beginning of the resultant code.<br/>
6.Write the result to an output binary file, which will be our compressed file.<br/>

## Decompression
1.Read binar file<br/>
2.Read padding information. Remove the padded bits<br/>
3.Decode the bits - read the bits and replace the valid Huffman Code bits with the character output<br/>
4.Save the decoded data to output file<br/>

![Screenshot (32)](https://user-images.githubusercontent.com/71879662/110785272-c233ac80-8290-11eb-8041-d623d806f70b.png)
![Screenshot (33)](https://user-images.githubusercontent.com/71879662/110785276-c364d980-8290-11eb-8123-104301e7f5c8.png)
![Screenshot (34)](https://user-images.githubusercontent.com/71879662/110785281-c3fd7000-8290-11eb-86e9-4d1ab0f59113.png)
![Screenshot (35)](https://user-images.githubusercontent.com/71879662/110785284-c4960680-8290-11eb-91bf-f4b9a0fe6655.png)
![Screenshot (36)](https://user-images.githubusercontent.com/71879662/110785287-c52e9d00-8290-11eb-88ae-5de4d033b811.png)





