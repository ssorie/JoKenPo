# JoKenPo
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Drawing.Text;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace JoKenPo
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }


        private void label1_Click(object sender, EventArgs e)
        {
            int lblplayer1;
            enum Escolhas { Pedra, Papel, Tesoura}
            Escolhas[] escolhas = { Escolhas.Pedra, Escolhas.Papel, Escolhas.Tesoura };
            Escolhas jogadorEscolha, IAEscolha;

        private void lblplayer2_Click(object sender, EventArgs e)
        {
            int lblplayer2;
            enum Escolhas { Pedra, Papel, Tesoura }
        Escolhas[] escolhas = { Escolhas.Pedra, Escolhas.Papel, Escolhas.Tesoura };
        Escolhas jogadorEscolha, IAEscolha;
        }        

        private void Escolhas_Clicl(object sender, EventArgs e)
        {
            PictureBox pic = (PictureBox)sender;
            if (pode jogar)
                    {
                switch (pic.Tag.ToString);
                {
                    Case "pedra": jogadorEscolha = Escolhas.Pedra; pbJogador.Image = Proprieties.Resource.rock; break;
                    Case "papel": jogadorEscolha = Escolhas.Papel; pbJogador.Image = Proprieties.Resource.paper; break
                    Case "tesoura": jogadorEscolha = Escolhas.Tesoura; pbJogador.Image = Proprieties.Resource.scissors; break
                }
                podeJogar = false;
                JogadaIA;
            }

        }

        private void JogadaIA()
        {
            Random rdn = new Random();
            IAEscolha = escolhas[rdn.Next(0, escolhas.length)];

            switch (IAEscolha.ToString()) {
                Case "pedra": jogadorEscolha = Escolhas.Pedra; pbJogador.Image = Proprieties.Resource.rock; break;
            Case "papel": jogadorEscolha = Escolhas.Papel; pbJogador.Image = Proprieties.Resource.paper; break
                    Case "tesoura": jogadorEscolha = Escolhas.Tesoura; pbJogador.Image = Proprieties.Resource.scissors; break
                }
        switch (jogadorEscolha.ToString()){
        case "Pedra": ChecarPedra(); break;
        case "Papel": ChecarPapel(); break;
        case "Tesoura": ChecarTesoura(); break;
    }

        private void ChecarPedra()
{
    switch (IAEscolha.ToString())
    {
        case "Pedra": MessageBox.Show("Empate!"); break;
        case "Papel": MessageBox.Show("Você perdeu!"); break;
            lblplayer2++; lblIA.Text = "CPU: " + lplplayer2.ToString(); break;
        case "Tesoura": MessageBox.Show("Você ganhou!");
            lplplayer1++; lbljogador.Text = "P1: " + lplplayer1.ToString(); break;
    }
    podeJogar = true; pbIA.Image = null; pbJogador.Image = null;
}

private void ChecarPapel()
{
    switch (IAEscolha.ToString())
    {
        case "Pedra": MessageBox.Show("Empate!"); break;
        case "Papel":
            MessageBox.Show("Você perdeu!"); break;
            lblplayer2++; lblIA.Text = "CPU: " + lplplayer2.ToString(); break;
        case "Tesoura":
            MessageBox.Show("Você ganhou!");
            lplplayer1++; lbljogador.Text = "P1: " + lplplayer1.ToString(); break;
    }
    podeJogar = true; pbIA.Image = null; pbJogador.Image = null;
}

private void ChecarTesoura()
{
    switch (IAEscolha.ToString())
    {
        case "Pedra": MessageBox.Show("Empate!"); break;
        case "Papel":
            MessageBox.Show("Você perdeu!"); break;
            lblplayer2++; lblIA.Text = "CPU: " + lplplayer2.ToString(); break;
        case "Tesoura":
            MessageBox.Show("Você ganhou!");
            lplplayer1++; lbljogador.Text = "P1: " + lplplayer1.ToString(); break;
    }
    podeJogar = true; pbIA.Image = null; pbJogador.Image = null;
}


