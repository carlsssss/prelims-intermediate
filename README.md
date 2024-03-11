using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace formidterm
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void Form1_Load(object sender, EventArgs e)
        {
            cbSelect.Items.Add("Apple");
            cbSelect.Items.Add("Banana");
            cbSelect.Items.Add("Orange");
        }

        private void radioButton1_CheckedChanged(object sender, EventArgs e)
        {

        }

        private void cbSelect_SelectedIndexChanged(object sender, EventArgs e)
        {

        }

        private void btnok_Click(object sender, EventArgs e)
        {
            if (cbSelect.SelectedItem.ToString() == "Apple")
            {
                MessageBox.Show("Ang pinili mo ay Apple 10 pesos");
            }
            else if (cbSelect.SelectedItem.ToString() == "Banana")
            {
                MessageBox.Show("Ang pinili mo ay Banana 15 pesos");
            }
            else if (cbSelect.SelectedItem.ToString() == "Orange")
            {
                MessageBox.Show("Ang pinili mo ay Orange 20 pesos");
            }
        }

        private void btnGender_Click(object sender, EventArgs e)
        {
            if (rbMale.Checked)
            {
                MessageBox.Show("Ikaw ay Lalake");
            }
            else if (rbFemale.Checked)
            {
                MessageBox.Show("Ikaw ay Babae");
            }

        }
    }
}
