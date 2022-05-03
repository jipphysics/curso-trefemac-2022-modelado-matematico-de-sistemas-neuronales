# Tutorial: Instalar  **conda** y **jupyter** en  **Linux** (Ubuntu/Debian)

A lo largo del curso utilizaremos **notebooks** de **Juypyer/Python** en [Google Colab](https://colab.research.google.com). Alternativamente, podemos utilizar **notebooks** de **Jupyter/Python** en nuestra laptop/desktop luego de instalar **miniconda**, una versión minimalista del administrador de entornos y paquetes llamado [Conda](https://docs.conda.io/en/latest/).

1. Para instalar **miniconda** en su **sistema operativo**, bájese el instalador correspondiente de

  [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)
  
En nuestro caso, **Ubuntu/Linux** de 64bits, bajaremos el que dice [Miniconda3 Linux 64-bit](https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh).

2. Vaya a la carpeta en donde se descargó el archivo `Miniconda3-latest-Linux-x86_64.sh`, y ejecute en una terminal (o consola bash) el comando

        $ bash Miniconda3-latest-Linux-x86_64.sh`
        
y acepte todo lo que sea necesario para completar la instalación. Esto generará en su **home** un directorio llamado `miniconda3`.

3. Active el entorno conda ingresando el comando

        $ source miniconda3/bin/activate
        
Luego, `(base)` debería aparecer en el prompt de su terminal, indicando que el entorno base de conda se ha activado.
        
4. Con el **entorno base activado**, instalaremos varios paquetes de **Python**, incluyendo el de **Jupyter** para ejecutar **notebooks**.

  - Instalamos el paquete **Jupyter** ingresando el comando
  
        (base) $ conda install -c anaconda jupyter 
  
  - Instalamos el paquete **matplotlib** ingresando el comando
  
        (base) $  conda install -c conda-forge matplotlib
        
        
  - Instalamos el paquete **numpy** ingresando el comando
  
        (base) $  conda install -c numpy
        
        
  - Instalamos el paquete **scipy** ingresando el comando
  
        (base) $  conda install -c scipy
        
5. Para iniciar un administrador de **notebooks** de **Jupyter**, escribir en una terminal

        (base) $ jupyter notebook
  
y el administrador de notebooks de Jupyter debería abrirse en su navegador web configurado por defecto.
