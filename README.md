# opencsv
Use C++ to read CSV files, including obtaining the number of rows and columns and specifying the data of a row or a column.

//this->row //the number of rows

//this->col //the number of columns //return int

//this->getRow(r) //obtaining the data from a row (index from zero)

//this->getCol(c) //obtaining the data from a column (index from zero) //return the pointer of vector

//csv must be saved as GBK coding form 

For example:
  
    CsvFile Csv("./data.csv");
    //obtain the number of rows and columns of the csv file
    cout<<"There is"<<Csv.row<<"rows"<<endl;
    cout<<"There is"<<Csv.col<<"columns"<<endl;

    //read the data from the first column of the csv file
    vector<string>* v=NULL;
    v=Csv.getCol(0);
    //print the data in vector
    for(int i=0;i<v->size();i++)
    {
        cout<<(*v)[i]<<endl;
    }
    system("pause");
    return 0;

More detail introduction can be available in https://www.bilibili.com/video/BV1yP4y1w7FE.
