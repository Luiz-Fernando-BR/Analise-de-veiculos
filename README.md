# **Veículos Detecção com OpenCV**

Este projeto utiliza a biblioteca OpenCV para realizar a detecção de veículos em vídeos. A detecção é feita através de um classificador em cascata (Haar Cascade) treinado, permitindo identificar veículos automaticamente em qualquer sequência de vídeo fornecida. O projeto é ideal para automação de tarefas de monitoramento de tráfego ou sistemas de segurança.

## **Tecnologias Utilizadas**
- **Python**: 3.12.4
- **OpenCV**: Biblioteca de visão computacional usada para processamento de imagens e vídeos.
- **Cascade Classifier**: Técnica de aprendizado supervisionado usada para detectar objetos em imagens, neste caso, veículos.
- **Biblioteca de Visão Computacional**: https://docs.opencv.org/3.4/db/d28/tutorial_cascade_classifier.html
  
## **Funcionalidades**
- Leitura de arquivos de vídeo (MP4 ou outros formatos compatíveis).
- Detecção em tempo real de veículos em cada frame do vídeo.
- Desenho de caixas delimitadoras ao redor dos veículos detectados.
- Interface interativa para visualização dos resultados.
  
## **Como Usar**

1. **Clone o Repositório**:
   ```bash
   git clone https://github.com/SEU_USUARIO/VEICULOS_DETECACAO.git
   ```

2. **Instale as Dependências**:
   Certifique-se de que você tem o Python 3.x instalado e, em seguida, instale as dependências necessárias:
   ```bash
   pip install opencv-python opencv-contrib-python
   ```

3. **Prepare os Arquivos**:
   - Coloque o vídeo de entrada (`carv.mp4`) e o arquivo XML do classificador Haar (`carx.xml`) no diretório do projeto.
   
4. **Execute o Código**:
   Execute o script Python, fornecendo os caminhos para o vídeo e o classificador Haar como argumentos:
   ```bash
   python Vehicles_detection.py -v "caminho/do/vídeo" -x "caminho/do/classificador.xml"
   ```

5. **Resultado**:
   O script irá abrir uma janela com o vídeo, onde os veículos detectados serão destacados com retângulos vermelhos. Pressione **ESC** para fechar a janela e interromper a execução.

## **Exemplo de Uso**
```bash
python Vehicles_detection.py -v "C:\caminho\para\carv.mp4" -x "C:\caminho\para\carx.xml"
```

## **Estrutura do Projeto**
- `Vehicles_detection.py`: Script principal que realiza a detecção de veículos.
- `carv.mp4`: Exemplo de vídeo a ser utilizado para a detecção.
- `carx.xml`: Arquivo Haar Cascade pré-treinado para detectar veículos.
