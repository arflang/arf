## Comments
```c
/* 
 * Multi
 * Line
 * Comment 
 */

// one line comment
```

## Functions
```c

// infix function
// min(1, 2)
// or
// 1 `min` 2
#f.infix min(x, y: Int): Int {
    if x > y then x else y
}

// lambda function
#f ...
#f: Int ...
#f (x, y: Int): Int ...
#f [T](x, y): T ...
#f [T](x, y): Int ...

// private and implicit function definition
#f.private
  .implicit sum[T](x, y: T): T ...

// implicit function definition
#f.implicit sum[T](x, y: T): T ...

// private function definition
#f.private sum[T](x, y: T): T ...

// public function definition
// or you can write explicitly .public
// #f.public sum[T](x, y: T): T ...
#f sum[T](x, y: T): T ...

// polymorphic function definition
#f sum[T](x, y: T): T {
    // return
    x + y
}

// monomorphic function definition
#f sum(x, y: Int): Int {
    // return
    x + y
}

// main function definition
#f main(args: String*) {

} 
```

## Object (or Classes)
```c
#o Point {
    // immutable properties
    val x, y: Int

    // immutable and private properties
    val.private x, y: Int

    // mutable properties
    var x, y: Int

    // mutable and private properties
    var x, y: Int

    // mutable and private properties with getter
    var.getter x, y: Int

    // private constructor
    #.private() {}

    // public constructor
    #() {}

    // constructor overloading
    #(x: Int) {}
    #(p: (Int, Int)) {}
    #(x, y: Int) {}
} 
```

## Data (or Case classes, data classes)
```c
#d Point {
    // immutable after set
    val x, y: Int
}
```
