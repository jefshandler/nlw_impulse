## Usaremos o Expo
npm install -g expo-cli

## Comando para Criar aplicação
expo init {nome da aplicação} nosso caso mobile

## escolhemos a opção template blank typescript

## Comando para configurar fontes
expo install expo-font @expo-google-fonts/inter

## Temos 2 opções para a lib do carregamento automatico da pagina 
# expo install expo-app-loading
## e 
# expo install expo-splash-screen
#para splash ---->
SplashScreen.preventAutoHideAsync();
  const [fontsLoaded] = useFonts({
    Inter_400Regular,
    Inter_500Medium,
  });

  if (!fontsLoaded) {
    return null;
  }

  SplashScreen.hideAsync();
#
# vai depender da versao do Expo instalada

# Instalar biblioteca de icones Phosphor
npm install --save phosphor-react-native
# Instalar biblioteca para trabalhar com SVG
expo install react-native-svg
# biblioteca para lidar com iphone
npm install react-native-iphone-x-helper
# biblioteca para lidar com abrir barra (gestos) MENU -- MODAL
expo install @gorhom/bottom-sheet@^4
# biblioteca de Dependencias da Gorhom
expo install react-native-reanimated react-native-gesture-handler
# colocar esta linha no babem.json
plugins: ['react-native-reanimated/plugin'],
# colocar esta linha na primeira linha projeto
import 'react-native-gesture-handler';

## como boa pratica aposta a instalações destas Bibliotecas executar
expo start --clear

# biblioteca para lidar com screenshot 
expo install react-native-view-shot

import { captureScreen } from react-native-view-shot
# biblioteca para trabalhar com requiziçoes HTTP AXIOS
npm install axios
