# hoisting

### **Question 1**

console.log("bar:", bar) //"bar:", undefined

bar=15

var foo=1

console.log(foo, bar) //1, 15

var bar

### **Question 2**

var foo=5

console.log("foo:", foo) //"foo:", 5

var foo;

var bar=10;

var bar;

console.log("bar:", bar) //"bar:", 10

var baz=10

var baz=12

console.log("baz:", baz) //"baz:", 12

### **Question 3**

function foo(){

    function bar(){
    
        return 5
        
    }

    return bar()
    
    function bar(){
    
        return 10
        
    }
    
}

console.log(foo()) //10

### **Question 4**
