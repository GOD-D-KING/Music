#include "mainwindow.h"
#include "ui_mainwindow.h"
#include <windows.h>
#include <string>
#include <iostream>


MainWindow::MainWindow(QWidget *parent) :
    QMainWindow(parent),
    ui(new Ui::MainWindow)
{
    ui->setupUi(this);
}

MainWindow::~MainWindow()
{
    delete ui;
}

void MainWindow::on_toolButton_clicked()
{

}

void MainWindow::on_PLAY_clicked()
{
   QMediaPlayer* player = new QMediaPlayer;

    player ->setMedia(QUrl::fromLocalFile(FileName));

    player->play();
}

void MainWindow::on_OPEN_clicked()
{

    FileName = QFileDialog::getOpenFileName(this,"Open my file");
    if(!FileName.isEmpty())
    {
        ui->lineEdit->setText(FileName);
    }
}


