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
                    println "El resultado de la multiplicación es: " + mult
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
                    println "El resultado de la potencia es: " + potencia
                }
            }
        }
    }
}
