#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;

int main() {
    srand(time(0));

    int randomSon = rand() % 100 + 1;
    int taxmin;
    int urinish = 0;

    cout << "=== SON TOPISH O'YINI ===" << endl;
    cout << "1 dan 100 gacha son o'ylangan." << endl;

    do {
        cout << "Son kiriting: ";
        cin >> taxmin;

        urinish++;

        if (taxmin > randomSon) {
            cout << "Kichikroq son kiriting!" << endl;
        }
        else if (taxmin < randomSon) {
            cout << "Kattaroq son kiriting!" << endl;
        }
        else {
            cout << "TABRIKLAYMAN!" << endl;
            cout << "Siz sonni topdingiz!" << endl;
            cout << "Urinishlar soni: " << urinish << endl;
        }

    } while (taxmin != randomSon);

    return 0;
}
