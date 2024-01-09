#include <iostream>

using namespace std;

void tersYazdir(char* ptr) {
    if (*ptr == '\0')
        return;
    else {
        tersYazdir(ptr + 1);
        cout << *ptr;
    }
}

int main() {
    char dizi[] = "Merhaba";
    char* ptr = dizi;

    tersYazdir(ptr);

    return 0;
}
