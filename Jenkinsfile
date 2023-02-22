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
                    resM="El resultado de la multiplicación es: " + mult
                    println resM
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
                    resP="El resultado de la potencia es: " + potencia
                    println resP
                    res=data+"\n"+resP
                    writeFile(file: "salida.txt", text: res)
                }
            }
        }
    }
}
