import { View, Text, StyleSheet, Image, TextInput, TouchableOpacity } from "react-native";

export default function index() {
  return (
    <View style={styles.container}>
      <View style={styles.containerLogo}>
        <Image style={styles.logo} source={require('../assets/logo-pra-fazer.png')}></Image>
      </View>
      <TextInput placeholder="E-mail" style={styles.campos}>
      </TextInput>
      <TextInput placeholder="Senha" style={styles.campos}>
      </TextInput>
      <TouchableOpacity style={styles.botao}>
        <Text style={styles.txtBotao} >Entrar</Text>
      </TouchableOpacity>
      <TouchableOpacity>
        <Text style={{ color: 'white', textAlign: 'center' }}>Criar Usuário</Text>
      </TouchableOpacity>
    </View>
  )
}

const styles = StyleSheet.create({
  container: {
    backgroundColor: '#FF6600',
    flex: 1, //para setar o background na pagina inteira
  },

  containerFont: {
    color: 'blue',
    fontSize: 50
  },

  logo: {
    width: 230,
    height: 40
  },

  containerLogo: {
    marginBottom: 50,
    height: 100,
    paddingTop: 250,
    paddingBottom: 10,
    alignItems: 'center',
  },

  campos: {
    backgroundColor: 'white',
    padding: 15,
    marginVertical: 8,
    marginHorizontal: 30,
    borderRadius: 10
  },

  botao: {
    backgroundColor: '#070A52',
    padding: 15,
    marginVertical: 8,
    marginHorizontal: 30,
    borderRadius: 10,
    marginBottom: 15
  },

  txtBotao: {
    color: 'white',
    textAlign: 'center',
    fontSize: 20
  }
})
