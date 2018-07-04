# Database Version 2
  * เพิ่มฟิลด์ Buniness Type, Company ในส่วน Working //nancy
  * เก็บฟิลด์ Working, Residence เป็น array //toto 
  * เพิ่มฟิลด์ CardStatus เพื่อบอกสถานะ public หรือ private ในส่วน CardList //toto
  * เพิ่มฟิลด์ Profile เก็บรายละเอียด Image,Status,Description,UpdateDTM //kelly and riya
  
  
# Todo/Issue
   * เปลี่ยนชื่อ field Contacts และ Contact List เพื่อให้สื่อความหมายที่เข้าใจง่าย //toto
   * ออกแบบ collection สำหรับเก็บข้อมูล business type ในรูปแบบของ master //kelly
   * ดูเรื่องของการตั้งชื่อฟิลด์ที่สื่อความหมาย //kelly
   * ดูเรื่องการเข้าถึงข้อมูลและการอัพเดทข้อมูลที่ง่าย //kelly
   * ดูเรื่องความรวดเร็วในการค้นหาข้อมูล //kelly
   
   

Document Structure

```json
[
    {
     "AccountId": 1,         
     "FirstName": "ไพบูลย์",
     "LastName": "ยืนยง" ,
     "NickName": "เคล",
     "Working": [
                    {
                        "Company": "บริษัท ทรู คอร์ปอเรชั่น จำกัด (มหาชน)",
                        "Position" : "Senior System Analyst",
                        "Department": "Enterprise Service Development",
                        "Address": " 18 อาคาร บริษัท ทรู คอร์ปอเรชั่น จำกัด (มหาชน)ทรู ทาวเวอร์ ถนนรัชดาภิเษก แขวงห้วยขวาง เขตห้วยขวาง กรุงเทพฯ 10310",
                        "BusinessType": "Telecommunication",
                        "Latitude": 13.12024,
                        "Longitude": 100.12344
                    },
                    {
                        "Company": "Simple Corporation",
                        "Position": "Managing Director",
                        "Address": "36/235 หมู่บ้านพฤกษาวิลเลจ 29 ต.คลองสาม อ.คลองหลวง จ.ปทุมธานี 12120",
                        "BusinessType": "System Integration",
                        "Latitude": 13.12024,
                        "Longitude": 101.12344
                    }
                ],
     "Residence": [
                    {
                        "Address": "36/235 หมู่บ้านพฤกษาวิลเลจ 29 ต.คลองสาม อ.คลองหลวง จ.ปทุมธานี 12120",
                        "Latitude": 11.12024,
                        "Longitude": 101.12344
                    }
                  ],
     "School":["ชุมชนบ้านอ่าวลึกเหนือ","อ่าวลึกประชาสรรค์","นวมินทราชูทิศ ทักษิณ"],
     "University": ["สงขลานครินทร์"],
     "Skill": ["React","Nodejs","MongoDB"],
     "WebSite": "http://www.simple.com",
     "Profile": {
                    "Image":"asxcnrhvxe.png",
                    "Status":"การเดินทางคือการเรียนรู้",
                    "Description": "Life is easy. Why do we make it so hard.",
                    "UpdateDTM":"4/7/2561 21:57:23"
                },
     "LoginMethod":"UserId",
     "UserName": "Paiboo1",
     "Password": "5b3b28e401e0d3df00c4f3e6",
     "Contacts": {
                    "Phone": ["02-7654321"],
                    "Mobile": ["0864126585"],
                    "Email": 
                            [
                                "paiboon.yue@gmail.com",
                                "paiboon_yue@truecorp.co.th"
                            ],
                    "Facebook": ["paiboon yuenyong"],
                    "Line": ["kel303"],
                    "Instragrame": ["kel.py"],
                    "Twitter": ["py.kelly"]
                },      
    "ContactList":
                    [ 
                        {
                           "AccountId": 2
                        },
                        {
                            "AccountId": 3,
                            "Favorite": "Y",
                            "Note": "nancy account info"
                        },
                        {
                            "AccountId": 4,
                            "Favorite": "Y",
                            "Note": "toto account info"
                        },
                        {
                            "NickName": "Oak",
                            "FirstName": "Vorapon",
                            "LastName": "Thepa-amondech",
                            "HomePhoneNumber": "027890989",
                            "WorkPhoneNumber": "",
                            "MobileNumber":"",
                            "Email": "oak@gmail.com",
                            "Note": "",
                            "Favorite": "Y"
                        }
                    ] ,
        "CardList": 
                    [
                        {
                            "Name": "ไพบูลย์ ยืนยง",
                            "NameEN": "Paiboon Yuenyong",
                            "Position": "Senior System Analyst",
                            "Department": "Enterprise Service Development",
                            "Mobile": "+66 8 6412 6585",
                            "Company": "True Corporation",
                            "Phone": "+66 2661 6666",
                            "CardPattern": "1",
                            "CardStatus": "public" 
                         },
                         {
                            "Name": "Paiboon Yuenyong",
                            "Position": "Managing Director",
                            "Mobile": "0864126585",
                            "Company": "Simple Corporation",
                            "Phone": "02-7654321",
                            "CardPattern": "2",
                            "CardStatus": "private"
                        },
                        {
                            "Name": "Paiboon Yuenyong",
                            "Position": "Managing Director",
                            "Mobile": "0864126585",
                            "Company": "Simple Corporation",
                            "Phone": "02-7654321",
                            "FAX" : "+66 2661 6564",
                            "Email" : "paiboon.yue@gmail.com",
                            "Website": "www.simple.co.th",
                            "LineId": "kel303",
                            "Address": 
                                        { 
                                         "Building" : {
                                                        "Name": "AA Tower",
                                                        "Floor": "21",
                                                        "RoomNo": "80/399"
                                                      },
                                         "AddressNo": "123/35",
                                         "Soi": "Sukumvit 21",
                                         "Road": "Road (ASOK)",
                                         "SubDistrict": "North Klongtoey",
                                         "District": "Wattana",
                                         "Province": "Bangkok",
                                         "Postcode": "10100"
                                        },
                            "TaxId": "123456789012",
                            "Logo":"asxcnrhv.png",
                            "CardPattern": "2",
                            "CardStatus": "private"
                            
                        }
                    ]
    }
]

```
