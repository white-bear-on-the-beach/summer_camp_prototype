# Prototyp gry na potrzeby Summer Camp 2021

Wrzutka zawiera gotową działającą paczkę wraz z assetami i skryptami.
Aby uruchomić grę wystarczy pobrać tą paczkę i otworzyć jako projekt w Unity,
jednak warto spróbować stworzyć projekt samodzielnie, po zaimportowaniu poniższych assetów.

* [Uruchomienie ProBuildera](#uruchomienie-probuildera)

### Napisane skrypty:
- PlayerMovement.cs
- MouseLook.cs

### Assety z Asset Store (https://assetstore.unity.com/)
* Conifers [BOTD]: https://assetstore.unity.com/packages/3d/vegetation/trees/conifers-botd-142076
* Grass Flowers Pack Free: https://assetstore.unity.com/packages/2d/textures-materials/nature/grass-flowers-pack-free-138810
* Outdoor Ground Textures: https://assetstore.unity.com/packages/2d/textures-materials/floors/outdoor-ground-textures-12555
* Terrain Tools Sample Asset Pack: https://assetstore.unity.com/packages/2d/textures-materials/nature/terrain-tools-sample-asset-pack-145808

+ ProBuilder:
Window > Package Manager > Packages: Unity Registry > Search: ProBuilder and install

## Materiały pomocnicze

#### Uruchomienie ProBuildera

 ![image](https://user-images.githubusercontent.com/78505993/124717871-d2d5f580-df05-11eb-9abc-3511906cd8dd.png)

* Utworzenie terenu

![image](https://user-images.githubusercontent.com/78505993/124718234-2ea07e80-df06-11eb-8262-e5e078209098.png)

* Formowanie terenu

![image](https://user-images.githubusercontent.com/78505993/124718470-6c050c00-df06-11eb-84cf-174bc6226b37.png)

Nakładanie tekstur
![image](https://user-images.githubusercontent.com/78505993/124718602-88a14400-df06-11eb-90e8-3c781a861564.png)

Analognicznie dla drzew i trawy
![image](https://user-images.githubusercontent.com/78505993/124718736-b1c1d480-df06-11eb-96d7-285186d8aa3a.png)


Utworzenie prototypu playera
Należy utworzyć nowy Empty Object - 'Create Empty' i nazwać go player
Mając wybrany obiekt Player, dodajemy Component 'Character Controller'
![image](https://user-images.githubusercontent.com/78505993/124719128-1aa94c80-df07-11eb-8be3-ec80d2de9d92.png)

Dodajemy do playera obiekt Cylinder, aby pojawił nam się Capsule Colider na naszym Playerze
Przenosimy Main Camera do obiektu Playera
Tworzymy Empty Object nazywając go groundCheck
![image](https://user-images.githubusercontent.com/78505993/124719469-7542a880-df07-11eb-9cbe-ea504fa1796b.png)

Resetujemy pozycję Main Camera i podnosimy na wysokość "oczu postaci"
![image](https://user-images.githubusercontent.com/78505993/124719699-b63abd00-df07-11eb-8444-91f92dfc2e06.png)

Obiekt groundCheck ustawiamy na dole postaci
![image](https://user-images.githubusercontent.com/78505993/124719783-cc487d80-df07-11eb-84d8-32951f111381.png)


Skryptowanie


Dodajemy skrpyt dla obiektu Player za pomocą Add Component
Skrypt znajduje się w lokalizacji Assets > PlayerMovement.cs w niniejszym repozytorium

Dodajemy nową warstwę "FirstPerson"
![image](https://user-images.githubusercontent.com/78505993/124720325-54c71e00-df08-11eb-8c3d-04b11797693a.png)

Podpinamy do skryptu wszystko tak jak poniżej
![image](https://user-images.githubusercontent.com/78505993/124720416-6c9ea200-df08-11eb-88da-10a566ebdd05.png)

Dodajemy skrypt Assents > MouseLook.cs dla Main Camera i podpinamy Playera, jak poniżej
![image](https://user-images.githubusercontent.com/78505993/124720555-9061e800-df08-11eb-9e74-597230f2e954.png)

