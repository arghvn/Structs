package main

// Go’s structs are typed collections of fields. They’re useful for grouping data together to form records.

import "fmt"

//This person struct type has name and age fields.

type person struct {
    name string
    age  int
}

func newPerson(name string) *person {

    //newPerson constructs a new person struct with the given name.

    p := person{name: name}
    p.age = 42
    return &p
}

//we can safely return a pointer to local variable as a local variable will survive the scope of the function

func main() {

    //This syntax creates a new struct.

    //we can name the fields when initializing a struct.

    //Omitted fields will be zero-valued.

    //An & prefix yields a pointer to the struct.

    //Access struct fields with a dot.

    //You can also use dots with struct pointers - the pointers are automatically dereferenced.

    fmt.Println(person{"Bob", 20})

    fmt.Println(person{name: "Alice", age: 30})

    fmt.Println(person{name: "Fred"})

    fmt.Println(&person{name: "Ann", age: 40})

    fmt.Println(newPerson("Jon"))

    s := person{name: "Sean", age: 50}
    fmt.Println(s.name)

    sp := &s
    fmt.Println(sp.age)

    sp.age = 51
    fmt.Println(sp.age)
}


// outputs: 

//{Bob 20}
//{Alice 30}
//{Fred 0}
//&{Ann 40}
//&{Jon 42}
//Sean
//50
//51