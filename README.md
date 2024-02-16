#include <i>
#include <cmath>using namespace std;
int main() {
    double size = 10
    char ch 'S';
    string message = "Happy Valentine' Day";

    for (double y = 0; y <= 2 * size; y++) {
        for (double x = 0; x <= 2 * size; x++) {
            double dist1 = sqrt(pow(x - size, 2) + pow(y - size, 2));
            double dist2 = sqrt(pow(x - size, 2) + pow(y - 3 * size, 2));

            if (dist1 < size || dist2 < size) {
                if (x == 0 || x == 2 * size || y == 0 || y == 2 * size) {
                    cout << ch;
                } else {
                    int idx = (int)(y / size * message.length());
                    if (x == size && y > size && y < 3 * size) {
                        cout << message[idx];
                    } else {
                        cout << " ";
                    }
                }
            } else {
                cout << " ";
            }
        }
        cout << endl;
    }
