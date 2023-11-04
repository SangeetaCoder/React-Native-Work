# React-Native-Work
learn react native 
//props and styling
import Reac from 'react';
import { StyleSheet, Text, View, } from 'react-native';
// import { useState } from 'react';
 import Exstyles from './style'
const App = () => {   
  // const [name,setName]=useState("Sangeeta"); 
  // let data="Sam";

  // function testName(){
  //   data ="peter";
  //   setName("shrivas")
   // }
// let name ="Peter";
// const [name, setName]=useState("Arun")
    
  return (
    <View>                                          
      <Text style={ styles.textBox } >Style in React Native</Text>
      <Text style={{ fontSize: 30, color:'red', backgroundColor:'green'}} >Style in React Native</Text>
      <Text style={styles.textBox} >Style in React Native</Text>
      <Text style={styles.textBox} >Style in React Native</Text>
      <Text style={[ styles.textBox,Exstyles.textBox,{marginTop:20}]} >Style in React Native</Text>
      {/* <Button title='Update Props' onPress={()=>setName("Peter")} />
      <User name={name} age={29} /> */} 
      {/* <Text style={{ fontSize: 30}} >{data}</Text> */}
      {/* <Button title='Update Name' onPress={testName} /> */}
     
      </View>
  );
};

const styles=StyleSheet.create({
  textBox:{
    color:'#fff',
    fontSize:30,
    backgroundColor:'blue',
    marginBottom:10,
    padding:10,
    borderRadius:10,
    height:100,
    textAlignVertical:'center',
    textAlign:'center',
    borderColor:'red',
    borderWidth:2

  }
})

// const User=(props)=>{
//   // console.warn(props.name)
//   return (
//     <View style={{backgroundColor:'green' , padding:5}}> 
//     <Text style={{fontSize:30}}>Name : {props.name}</Text>
//     <Text style={{fontSize:30}}>Age : {props.age}</Text>
//     </View>
//   );
// }

// // {/* const UserData = () => {
// return(
//   <View>
//     <Text style={{fontSize:30}}>Name : Shivam</Text>
//     <Text style={{fontSize:30}}>Age : 100</Text>
//     <Text style={{fontSize:30}}>Email : sangeeta@test.com</Text>
//   </View>
// )
// } */}


export default App;

