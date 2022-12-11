# Week-5-Programming
Week 5 Programming Code

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Module5Project
{
    public partial class Form1 : Form
    {


        public Form1()
        {
            InitializeComponent();
        }







       
       

        private void button2_Click(object sender, EventArgs e)
        {

            int Low = int.Parse(textBox1.Text);
            int High = int.Parse(textBox2.Text);
            int Value = int.Parse(textBox3.Text);

            if (Low == Value || High == Value) //The program will check to see if the value is equal to one of the end values
            {
                label5.Text = "The value is equal to one of the range end points.";

            }
            else if (Value < Low) //The program will check to see if the Value is smaller than the Low end point
            {
                label5.Text = "The value is less than the low end point.";

            }
            else if (Value > High) //The program will check to see if the Value is higher than the High end point
            {
                label5.Text = "The value is greater than the high end point.";
            }

            else if ((Value > Low) && (Value < High)) //The program will check to see if the Value is in between both of the end points
                    {
                      label5.Text = "The value is in between the end points";
                    }


        }

        private void button1_Click(object sender, EventArgs e)
        {
            
                textBox1.Text = "";
                textBox2.Text = "";
                textBox3.Text = "";
                label5.Text = "";

            
        }

        private void button3_Click(object sender, EventArgs e)
        {
            
                this.Close();
            

        }
    }
}
//Ryan Bain
//Object Oriented Using C#
//10-13-2022
