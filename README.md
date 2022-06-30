# WE-Theory_React

# WE-Theory-React

STATE VS PROPS


State :

1. State is a inside the component
2. It will Re-Render that component while change in state.
3. state is a one type of function.
4. for example: In Counter App we use :

const [Count, setCount] = useState(0);
so initial value is 0 here.
now,
setCount(count + 1 )
so, now the counter will display 1.

Props :

1. Props We pass to the component from one to other component. We can also pass state function as props.
2. Props are mainly use for display and pass functionality to other components.
3. Props is always an object when the component recived it.
4. We can pass many things as props such as : number,string, function, array,object etc..
5. For example: 

<Child  name={name} handleClick={handleClick}   />

useState API :

1. It is inbuild Hook from the react.
2. It is managed to use the state of changing variable.
3. It is same works as a function.
4. It will take some initial value. const[state, setState] = useState(0); 
5. We can change that value by setState(state+1)

MAP : 

map function returns the value
const array1 = [1, 3, 9, 4];
const map1 = array1.map((a,i) =>{
    <div>{a * a}</div>
});

console.log(map1);
// expected output: Array [1, 9, 81, 16]


Filter :

let str = ["raju","shyam","baburao","ganpatrao"]
const delete = words.filter( (word, index, arr) => {
  arr.pop()
  return str.length < 6
})

console.log(deleteWords);
// expected output: str ["baburao","ganpatrao"]


Reduce :

const array1 = [1, 2, 3, 4];
const initialValue = 0;
const sumWithInitial = array1.reduce(
  (previousValue, currentValue) => previousValue + currentValue,
  initialValue
);

console.log(sumWithInitial);
