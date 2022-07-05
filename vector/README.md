Vectors are the same as dynamic arrays with the ability to resize itself automatically when an element is inserted or deleted, with their storage being handled automatically by the container.

Vector elements are placed in contiguous storage so that they can be accessed and traversed using iterators.
### Importing header file
```c++
	#include<vector.h>    // or #include<bits/stdc++.h>
```

## Creating vector
```c++
	vector<T> name;        //Where T -> type of the vector(int, char, string, float)
				 	//and name is the name of the vector

```

### Methods in vector
#### 1. push_back(value)
push_back(value) – It push the elements into a vector from the back

#### 2. at(position)
at(pos) – Returns a reference to the element at position ‘pos’ in the vector

#### 3. size()
size() – Returns the number of elements in the vector.


```c++
	vector<int> v;
	
	v.push_back(10);
	v.push_back(20);
	v.push_back(30);
	v.push_back(40);
	v.push_back(50);
	
	for(int i=0;i<v.size();i++){
		cout<<v[i]<<" ";
	}									//Output: 10 20 30 40 50
	cout<<endl;
	
	for(int i=0;i<v.size();i++){
		cout<<v.at(i)<<" ";
	}									//Output : 10 20 30 40 50
	cout<<endl;
```

#### 4. pop_back()
pop_back() – It is used to pop or remove elements from a vector from the back.
```c++
	vector<int> v;
	
	v.push_back(10);
	v.push_back(20);
	v.push_back(30);
	v.push_back(40);
	
	
	for(int i=0;i<v.size();i++){
		cout<<v.at(i)<<" ";
	}									//Output : 10 20 30 40
	cout<<endl;
	
	v.pop_back();
	v.pop_back();
	
	for(int i=0;i<v.size();i++){
		cout<<v.at(i)<<" ";
	}									//Output : 10 20
	cout<<endl;
```

#### 5. insert(pos, value)
insert() – It inserts new elements before the element at the specified position

```c++
	vector<int> v;
	
	v.push_back(10);
	v.push_back(20);
	v.insert(v.begin(), 30);
	v.insert(v.begin()+2, 40);
	
	
	for(int i=0;i<v.size();i++){
		cout<<v.at(i)<<" ";
	}									//Output : 30 10 40 20
	cout<<endl;
```
#### 6. emplace()
emplace() – It extends the container by inserting new element at position

#### 7. emplace_back()
emplace_back() – It is used to insert a new element into the vector container, the new element is added to the end of the vector

#### 8. clear()
clear() – It is used to remove all the elements of the vector container

#### 9. empty()
empty() – Returns whether the container is empty.

```c++
	vector<int> v;
	
	v.push_back(10);
	v.push_back(20);
	v.push_back(30);
	v.push_back(40);
	
	cout<<v.empty()<<endl;           //Output : 0  (means False)
	v.clear();
	
	cout<<v.empty()<<endl;          //Output : 1 (means True)
```

#### 10. erase() 
erase() – It is used to remove elements from a container from the specified position or range.

#### 11. reseize(n)
resize(n) – Resizes the container so that it contains ‘n’ elements.

```c++
	vector<int> v;
	
	cout<<v.size()<<endl;        //Output : 0
	
	v.resize(10);
	
	cout<<v.size()<<endl;     //Output : 10
```

#### 12. assign(size, value)
assign() – It assigns new value to the vector elements by replacing old ones
```c++
	vector<int> v;
	
	for(int i=0;i<v.size();i++){
		cout<<v.at(i)<<" ";
	}                                    //Output : 
	
	v.resize(10);
	v.assign(v.size(), 5);
	
	for(int i=0;i<v.size();i++){
		cout<<v.at(i)<<" ";      
	}                                     //Output : 5 5 5 5 5 5 5 5 5 5

```

#### 13. reserve()
reserve() – Requests that the vector capacity be at least enough to contain n elements.

#### 14. front()
front() – Returns a reference to the first element in the vector

#### 15. back()
back() – Returns a reference to the last element in the vector

#### 16. begin()
begin() – Returns an iterator pointing to the first element in the vector

#### 17. end()
end() – Returns an iterator pointing to the theoretical element that follows the last element in the vector

#### 18. swap()
swap() – It is used to swap the contents of one vector with another vector of same type. Sizes may differ.


vectors in c++ : [https://www.geeksforgeeks.org/vector-in-cpp-stl/]
