# zsign-gui

## how to use

zsign compile：x86_64-w64-mingw32-g++ *.cpp common/*.cpp -o zsign.exe -I../mman-win32 -I../openssl/include/ -L../openssl -L../mman-win32 -lmman -lcrypto -lgdi32 -std=c++11 -DWINDOWS -m64 -static-libgcc --static

zsign-gui compile：pyinstaller -F -w -i p10.ico zsign-gui.py

ps：you need use dirent.h in the repo to replace mingw's dirent.h

reference: https://blog.csdn.net/a513436535/article/details/108539238