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
                }
            }
        }
    }
}
