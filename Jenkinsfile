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
                    resP="El resultado de la potencia es: " + potencia
                    append(file: "salida.txt", text: resP)
                }
            }
        }
    }
}
