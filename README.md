using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace WindowsFormsApp1
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void button1_Click(object sender, EventArgs e)
        {
            int gr1, gr2, gr3, total, ave;
;
            gr1 = int.Parse(textBox2.Text);
            gr2 = int.Parse(textBox3.Text);
            gr3 = int.Parse(textBox4.Text);

            total = gr1 + gr2 + gr3;
            ave = total / 4;

            textBox5.Text = total.ToString();
            textBox6.Text = ave.ToString();


            if (ave >= 96)
            {
                textBox7.Text = "1.00";
            }
            else if (ave >= 94)
            {
                textBox7.Text = "1.25";
            }
            else if (ave >= 91)
            {
                textBox7.Text = "1.50";
            }
            else if (ave >= 88)
            {
                textBox7.Text = "1.75";
            }
            else if (ave >= 85)
            {
                textBox7.Text = "2.00";
            }
            else if (ave >= 83)
            {
                textBox7.Text = "2.25";
            }
            else if (ave >= 80)
            {
                textBox7.Text = "2.50";
            }
            else if (ave >= 78)
            {
                textBox7.Text = "2.75";
            }
            else if (ave >= 75)
            {
                textBox7.Text = "3.00";
            }
            else if (ave < 75)
            {
                textBox7.Text = "INC";
            }
        }
    }
}
