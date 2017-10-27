#include<iostream>
using namespace std;

class Book{
	protected:
		string title;
		string author;

	public:
		void setBook(string,string);
		void displayBook(){
			cout<<"Nama Buku : "<<title<<"\n";
			cout<<"Nama Pengarang : "<<author<<"\n";
		};
};

void Book::setBook(string iTitle, string iAuthor){
	title = iTitle;
	author = iAuthor;
}

class Fiksi: public Book {
	public:
		int gradeRead;
		void setGrade(string, string, int);
		void displayFiksi(){
			cout<<"Tingkatan Pembaca : "<<gradeRead<<"\n";
		};
};

void Fiksi :: setGrade(string iTitle, string iAuthor, int iGrade){
	Book::setBook(iTitle,iAuthor);
	gradeRead = iGrade;
}

class nonFiksi : public Book{
	public:
		int savePage;
		void setPage(string, string, int);
		void displayNonFiksi(){
			cout<<"Jumlah Halaman : "<<savePage<<"\n";
		};
};

void nonFiksi :: setPage(string iTitle, string iAuthor, int iPage){
	Book::setBook(iTitle,iAuthor);
	savePage = iPage;
}

int main(){
	Book a;
	a.setBook("Harry Senin", "Atmaja");
	a.displayBook();
	
	cout<<"\n";
	Fiksi b;
	b.setBook("Harry Selasa", "Hardinata");
	b.displayBook();
	b.displayFiksi();
	
	cout<<"\n";
	nonFiksi c;
	c.setBook("Harry Rabu", "Bagas");
	c.displayBook();
	c.displayNonFiksi();
}
