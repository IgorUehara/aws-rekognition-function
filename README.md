# aws-rekognition-function

1ª Função - first_createCollection - O objetivo dela é criar uma collection onde serão armazenados os metadados das imagens que você deseja treinar, para que a IA do serviço consiga reconhecer posteriormente.

2ª Função - second_createIndex - O objetivo dela é extrair os metadados da imagem e indexar na collection, nessa função você pode salvar um id externo para conseguir por exemplo puxar de um banco de dados as informações sobre a pessoa reconhecida.

3ª Função - third_searchImage - O objetivo dela reconhecer a imagem ou não a pessoa da imagem. Esse serviço irá buscar dentro da collection alguma imagem que se assemelhe. É interessante setar um FaceMatchThreshold acima de 80% para que a confiabilidade do reconhecimento seja alto.
