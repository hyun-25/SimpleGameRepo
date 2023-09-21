# SFML ���̺귯�� ��ġ

## ������Ʈ 
https://www.sfml-dev.org/download/sfml/2.6.0/

## �ٿ�ε�
- C++ 17 : 2022 / 32��Ʈ

## ���� ���� 
```
-SimpleGame  - External - include
						- lib
			 - SimpleGame
			 - SimpleGame.sln
```

- SFML > include ��ü ����/���� => SimpleGame > External > include
- SFML > lib ��ü ����/���� => SimpleGame > External > lib
- SFML > bin ��ü ���� => SimpleGame > SimpleGame


## VS 2022 ȯ�� ����

- Solution Explorer > Drop Down Menu > Properties
- ��� ���� ����
  - Configuration > All Configuration
  - Platform> Win32
- C/C++ > General > Additional include Directories
  - SFML���� �����ؿ� ����/������ �ִ� ��ġ(����)�� ����
  - $(SolutionDir) : ���� ������Ʈ ���� 

- Linker > General > Additional Library Directories
	- SFML���� �����ؿ� ����/������ �ִ� ��ġ(����)�� ����

- Linker > Input > additional Dependencies
	- Configuration > Release
```
  sfml-system.lib 
  sfml-graphic.lib
  sfml-window.lib
  sfml-audio.lib
  sfml-network.lib 
```

- Linker > Input > additional Dependencies
	- Configuration > Debug
```
  sfml-system-d.lib 
  sfml-graphic-d.lib
  sfml-window-d.lib
  sfml-audio-d.lib
  sfml-network-d.lib 
```