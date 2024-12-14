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


# Crie o diretório do workspace
```
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/
```

# Inicialize o workspace com catkin
```
catkin_make
source devel/setup.bash
```

## Passo 2: Adicionando o Pacote ao Workspace

Clone este repositório no diretório src do seu workspace:

```
cd ~/catkin_ws/src
git clone https://github.com/seu_usuario/nome_do_repositorio.git
```

## Passo 3: Compilando o Pacote

Navegue até o diretório do seu workspace:
```
cd ~/catkin_ws
```
Compile o workspace usando o catkin_make:
```
catkin_make
source devel/setup.bash
```

## Passo 4: Executando os Scripts de Lançamento

Para lançar o robo no Gazebo, use o seguinte comando:
```
roslaunch my_robot_urdf spawn_urdf.launch
```
Para lançar o robo no RViz, use os seguinte comando:
```
roslaunch my_robot_urdf display.launch
```
