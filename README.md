# Mental-Health-App-BreakThrough
//Built a mental health app with XCode in the language Swift that will connect users to a chatbot built with IBM Cloud Watson 
import UIkit

class PickerViewController:UIViewController, UIPickerViewDelegate, UIPickerViewDataSource{
      @IBOutlet weak var pickerViewer2: UIPickerView!
      func numberOfComponents(in pickerview:UIPickerView)->Int{
      return 1
      }
      func pickerView(_pickerView:UIpickerView,numberOfRowsInComponent component:Int)->Int{
      
      
      return pickerData.cont
      }
      
      func pickerView(_pickerview:UIPickerView,titleForRow row:Int,forComponent component: Int)->String?{
            return pickerData[row]
           }
           
           @IBOutlet weak var pickView: UIPickerView!
           
    //INPUT THE DATA INTO THE ARRAY
    
    let pickerData = ["1","2","3","4","5"]
    let pickerData2 = ["1","2","3","4","5"]
    override func viewDidLoad(){
        super.viewDidLoad()
        
        //Connect data:
        
        self.pickView.delegate =self
        self.pickView.dataSource = self
        
        
        }
    
