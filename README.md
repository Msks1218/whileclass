# whileclass
//
//  ViewController.swift
//  VowelTester
//
//  Created by Manavarthi,Sanjay Krishna on 1/25/22.
//

import UIKit

class ViewController: UIViewController {

    @IBOutlet weak var textoutlet: UITextField!
    
    @IBOutlet weak var displayLable: UILabel!
    
    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view.
    }

    @IBAction func buttonClicked(_ sender: UIButton) {
        //read text, check whether given digit is vowel or not..
        var enteredtext=textoutlet.text!
        //checking vowel
        if
            (enteredtext.contains("a")) ||
             (enteredtext.contains("e")) ||
                (enteredtext.contains("i")) ||
                (enteredtext.contains("o")) ||
                (enteredtext.contains("u")) {
            displayLable.text="It has vowels"
        }
        else{
            displayLable.text="no vowels"
        }
    }
    
}

