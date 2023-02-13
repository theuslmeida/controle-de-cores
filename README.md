# controle-de-cores
import React, {useState} from "react";
import { View, Button, Text} from "react-native";

export default function Abacaxi(){
  const [red, setRed] = useState(0)
  const [green, setGreen] = useState(0)
  const [blue, setBlue] = useState(0)

  function vermelho(){setRed(red+10)}
  function azul(){setBlue(blue+10)}
  function verde(){setGreen(green+10)}

  return(
    <View style={{backgroundColor: "rgb("+red+","+green+","+blue+")", flex: 1}}>
      <Button title="RED"onPress={vermelho}/>
      <Button title="GREEN"onPress={verde}/>
      <Button title="BLUE"onPress={azul}/>
    </View>
  )
}
