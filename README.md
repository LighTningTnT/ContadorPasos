# ContadorPasos
Programa que me permite contar pasos 
#include <iostream>
#include <string>

class Persona {
public:
    Persona(const std::string &nombre, int edad)
        : nombre(nombre), edad(edad) {}

    void saludar() const {
        std::cout << "Hola, soy " << nombre << " y tengo " << edad << " años." << std::endl;
    }
private:
    std::string nombre;
    int edad;
};

int main() {
    std::string nombre;
    int edad;

    std::cout << "Ingrese el nombre y la edad: ";
    std::cin >> nombre >> edad;

    Persona persona(nombre, edad);
    persona.saludar();

    return 0;
}
