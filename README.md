# Grupo-8
# Projeto ROS Noetic

Este repositório contém um pacote ROS Noetic que pode ser adicionado ao diretório `src` de seu workspace e executado a partir dos scripts `launch`.

## Pré-requisitos

Antes de começar, verifique se você tem as seguintes ferramentas instaladas:

- [ROS Noetic](http://wiki.ros.org/noetic) (completo ou a versão que você precisa)
- [catkin](http://wiki.ros.org/catkin) (para compilar o workspace)
- Sistema operacional Ubuntu (recomendado)

### Instalando o ROS Noetic

Se você ainda não tem o ROS Noetic instalado, siga as instruções no [site oficial do ROS Noetic](http://wiki.ros.org/noetic/Installation/Ubuntu).

## Passo 1: Configuração do Workspace

Se você ainda não possui um workspace ROS, crie um novo workspace com os seguintes comandos:

```bash
# Crie o diretório do workspace
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/

# Inicialize o workspace com catkin
catkin_make
source devel/setup.bash
