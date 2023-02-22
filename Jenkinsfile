def a=5
def b=2
pipeline
{
    agent any
    stages
    {
        stage("Multiplicación")
        {
            steps
            {
                script
                {
                    def mult=a*b
                    resM="El resultado de la multiplicación es: " + mult+".\n"
                    writeFile(file: "salida.txt", text: resM)
                }
            }
        }
        stage("Potencia")
        {
            steps
            {
                script
                {
                    def suma=a+b
                    def potencia=suma*suma
                    def data = readFile(file: "salida.txt")
                    resP=data+"El resultado de la potencia es: " + potencia
                    writeFile(file: "salida.txt", text: resP)
                }
            }
        }
    }
}
