using System;
using System.Windows.Forms;
namespace WindowsFormsApplication1
{
	public partial class form1:form
	{
		public form1()
		{
			IntializeComponent();
		}
		private void dateTimePicker2_valueChanged(object sender,EventArgs e)
		{
			int d;
			DateTime firstdate=Convert.ToDateTime(DateTimePicker1.Text);
			DateTime seconddate=Convert.ToDateTime(DateTimepicker2.Text);
			d=firstdate.Subtract(seconddate).days;
			textbox1.Text=Math.Abs(d).ToString();
			
		}
	}
}
