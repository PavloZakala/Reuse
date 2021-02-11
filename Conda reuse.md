Встановити [Miniconda](https://docs.conda.io/en/latest/miniconda.html) 

Linux:
```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda.sh
bash ~/miniconda.sh -b -p ~/miniconda
echo "PATH=\$PATH:\$HOME/miniconda/bin" >> .bashrc
```

Створити нове conda/miniconda середовище Python 3.8
```bash
conda create -n myenv python=3.8
```

Експортувати conda/miniconda середовище в .yml файл
```bash
conda env export > environment.yml
```

Створити conda/miniconda середовище на основі .yml файлу
```bash
conda env create -f environment.yml
```

Видалити conda/miniconda середовище в .yml файл
```bash
conda remove --name myenv --all
```
