# Pairs and Iterators

Now we are going to start to look at associative data strucures. Unlike vectors, stacks, and queues, associative data structures are not stored in a particular order and cannot be accessed in an orderly fashion. Instead, they are accessed through keys and values as opposed to an index.

You can also access all the elements in an associative data structure by iterating through them, however since there is no index to access the values, you need to access in a different way using an iterator.

In this lesson, you are going to get a quick introduction to two elements that will be used to help with access to these associative data structures, pairs and iterators. You will then use these as you explore sets and maps later in the module.

## Pairs

A pair is exactly how it sounds, it is a pair of values. Pairs can be two values of the same type, but they can also contain values of a different type. Pairs are often used to hold two pieces of related data. You will see pairs used later in this module as you explore key/value pairs with maps.

### Creating Pairs

Pairs are part of the C++ standard library and do not need a special import statement.

To declare a pair, you use the keyword pair and specify the two types of variables inside angled brackets and then the variable name.

Basic Form:
```c++
pair<type1, type2> variableName;
```

Examples:
```c++
pair<string, string> address;
pair<string, int> nameAge;
pair<double, double> math;
```

When creating the pair, you can assign initial values by placing them inside curly brackets.

Examples:
```c++
pair<string, int> nameAge {"Karel", 9};
pair<double, double> math {5.3, 8.7};
```

### Accessing and Updating Values

Accessing and updating values is similar to how values are accessed and updated with a struct. With structs, you access the value with a dot and the member name. Since a pair doesn’t have member variables, you simply access using the keywords `first` and `second`.

Example:
```c++
pair<string, string> address {"Chicago", "IL"};

cout << address.first << endl;
cout << address.second << endl;
```
Output:
```
Chicago
IL
```
Updates are done using the same access.
```c++
pair<string, int> nameAge {"Karel", 9};
nameAge.second = 10;
```

### Using Pairs

Just like any other data structure, pairs can be used as a separate data structure or as part of another data structure. In this example, you can see how pairs can be used with a vector or a queue.

Examples:
```c++
vector<pair<string, int> > classRoster;
queue<pair<string, string> > names;
```
As mentioned above, pairs will be used for specific purposes in C++, like maps. Beyond that, pairs do have limited use since it can often be just as easy and more descriptive to create a struct. For example, if you wanted to store the first and last name, you can do this with a pair and then represent the first name in the first position and the last name in the second position.

Alternatively, you can create a `name` struct and give the member names more descriptive values such as firstName and lastName.