# Consulta_De_Cadastro



using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace cadastro
{
    public partial class Consulta__De_Cadastro : Form
    {
        public Consulta__De_Cadastro()
        {
            InitializeComponent();
        }

        private void bTnExibir_Click(object sender, EventArgs e)
        {
        //Criando Variaveis
            String Nome;
            String Sobrenome; 
            
            
          //Atribundo Valor
        
            Nome = Convert.ToString(txtNome.Text);
            Sobrenome = Convert.ToString(txtSobrenome.Text);
            
            //Mecanização do codigo

            if (RTSolteiro.Checked)
            {
                MessageBox.Show(Nome + " " + Sobrenome + " Solteiro(a)");
            }
            else if (RTCasado.Checked)
            {
                MessageBox.Show(Nome + " " + Sobrenome + " Casado(a)");

            }
            else if (RTDivorciado.Checked)
            {
                MessageBox.Show(Nome + " " + Sobrenome + " Divorciado(a)");
            }
            else if (RTViúvo.Checked)
            {
                MessageBox.Show(Nome + " " + Sobrenome + " Viúvo(a)");
            }
        }
    }
}
