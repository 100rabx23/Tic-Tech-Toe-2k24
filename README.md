# Tic-Tech-Toe-2k24

const districts = {
    andhraPradesh: [
        "Anantapur", "Chittoor", "East Godavari", "Guntur", "Krishna", 
        "Kurnool", "Nellore", "Prakasam", "Srikakulam", "Visakhapatnam", 
        "Vizianagaram", "West Godavari"
    ],
    arunachalPradesh: [
        "Anjaw", "Changlang", "Dibang Valley", "East Kameng", "East Siang", 
        "Kamle", "Kra Daadi", "Kurung Kumey", "Lepa Rada", 
        "Lower Dibang Valley", "Lower Subansiri", "Namsai", 
        "Pakke Kessang", "Papum Pare", "Siang", "Tawang", 
        "Tirap", "Upper Siang", "Upper Subansiri", "West Kameng", 
        "West Siang"
    ],
    assam: [
        "Baksa", "Barpeta", "Biswanath", "Bongaigaon", "Cachar", 
        "Charaideo", "Chirang", "Darrang", "Dhemaji", "Dibrugarh", 
        "Goalpara", "Golaghat", "Hailakandi", "Jorhat", "Kamrup", 
        "Karbi Anglong", "Karimganj", "Kokrajhar", "Lakhimpur", 
        "Morigaon", "Nagaon", "Nalbari", "Sivasagar", 
        "Sonitpur", "Tinsukia", "Udalguri", "West Karbi Anglong"
    ],
    bihar: [
        "Araria", "Arwal", "Aurangabad", "Banka", "Begusarai", 
        "Bhagalpur", "Buxar", "Darbhanga", "Gaya", "Gopalganj", 
        "Jamui", "Jehanabad", "Kaimur", "Katihar", "Khagaria", 
        "Madhepura", "Madhubani", "Nalanda", "Nawada", 
        "Patna", "Purnia", "Rohtas", "Saharsa", "Samastipur", 
        "Saran", "Sheikhpura", "Sheohar", "Sitamarhi", 
        "Siwan", "Supaul", "Vaishali", "West Champaran"
    ],
    chhattisgarh: [
        "Balod", "Baloda Bazar", "Bilaspur", "Dantewada", "Dhamtari", 
        "Durg", "Gariaband", "Janjgir-Champa", "Jashpur", "Kabirdham", 
        "Kanker", "Korba", "Kondagaon", "Mahasamund", "Raigarh", 
        "Raipur", "Rajnandgaon", "Surguja"
    ],
    goa: [
        "North Goa", "South Goa"
    ],
    gujarat: [
        "Ahmedabad", "Amreli", "Anand", "Banaskantha", "Bharuch", 
        "Bhavnagar", "Dahod", "Dangs", "Gandhinagar", "Jamnagar", 
        "Junagadh", "Kutch", "Mahisagar", "Mehsana", "Narmada", 
        "Navsari", "Panchmahal", "Patan", "Porbandar", 
        "Rajkot", "Sabarkantha", "Surat", "Surendranagar", 
        "Tapi", "Vadodara", "Valsad"
    ],
    haryana: [
        "Ambala", "Bhiwani", "Charkhi Dadri", "Faridabad", "Fatehabad", 
        "Gurugram", "Hisar", "Jind", "Kaithal", "Karnal", 
        "Mahendragarh", "Panchkula", "Panipat", "Rewari", 
        "Rohtak", "Sirsa", "Sonipat", "Yamunanagar"
    ],
    himachalPradesh: [
        "Bilaspur", "Chamba", "Hamirpur", "Kangra", "Kinnaur", 
        "Kullu", "Lahaul and Spiti", "Mandi", "Shimla", 
        "Sirmaur", "Solan", "Una"
    ],
    jharkhand: [
        "Bokaro", "Chatra", "Dhanbad", "Dumka", "East Singhbhum", 
        "Giridih", "Godda", "Gumla", "Hazaribagh", "Jamtara", 
        "Khunti", "Koderma", "Latehar", "Lohardaga", "Pakur", 
        "Palamu", "Ranchi", "Sahibganj", "Seraikela Kharsawan", 
        "Simdega", "West Singhbhum"
    ],
    karnataka: [
        "Bagalkote", "Ballari", "Belagavi", "Bengaluru", "Bidar", 
        "Chamarajanagar", "Chikkaballapur", "Chikmagalur", 
        "Chitradurga", "Dakshina Kannada", "Davanagere", "Dharwad", 
        "Gadag", "Hassan", "Haveri", "Kodagu", "Kolar", 
        "Koppal", "Mandya", "Mysuru", "Raichur", "Ramanagara", 
        "Shivamogga", "Tumakuru", "Udupi", "Uttara Kannada", 
        "Yadgir"
    ],
    kerala: [
        "Alappuzha", "Ernakulam", "Idukki", "Kollam", "Kottayam", 
        "Kozhikode", "Malappuram", "Palakkad", "Pathanamthitta", 
        "Thiruvananthapuram", "Thrissur", "Wayanad"
    ],
    madhyaPradesh: [
        "Agar Malwa", "Alirajpur", "Anuppur", "Ashoknagar", "Balaghat", 
        "Barwani", "Betul", "Bhopal", "Burhanpur", "Chhindwara", 
        "Dindori", "Guna", "Gwalior", "Harda", "Hoshangabad", 
        "Indore", "Jabalpur", "Jhabua", "Katni", "Khandwa", 
        "Khargone", "Mandla", "Mandsaur", "Morena", "Narmada", 
        "Neemuch", "Panna", "Rajgarh", "Ratlam", "Rewa", 
        "Sagar", "Satna", "Sehore", "Shahdol", "Shajapur", 
        "Sidhi", "Singrauli", "Tikamgarh", "Ujjain", 
        "Umaria", "Vidisha"
    ],
    maharashtra: [
        "Ahmednagar", "Akola", "Amravati", "Aurangabad", "Beed", 
        "Bhandara", "Buldhana", "Chandrapur", "Dhule", "Gadchiroli", 
        "Gondia", "Hingoli", "Jalna", "Kolhapur", "Latur", 
        "Mumbai", "Nagpur", "Nanded", "Nashik", "Osmanabad", 
        "Parbhani", "Pune", "Raigad", "Ratnagiri", "Sindhudurg", 
        "Solapur", "Thane", "Wardha", "Washim", "Yavatmal"
    ],
    manipur: [
        "Bishnupur", "Churachandpur", "Imphal East", "Imphal West", 
        "Jiribam", "Kakching", "Kamjong", "Kangpokpi", "Noney", 
        "Pherzawl", "Senapati", "Tamenglong", "Thoubal", "Ukhrul"
    ],
    meghalaya: [
        "East Garo Hills", "East Khasi Hills", "Jaintia Hills", 
        "North Garo Hills", "Ri Bhoi", "South Garo Hills", 
        "West Garo Hills", "West Khasi Hills"
    ],
    mizoram: [
        "Aizawl", "Champhai", "Kolasib", "Lawngtlai", "Lunglei", 
        "Mamit", "Saiha", "Serchhip"
    ],
    nagaland: [
        "Dimapur", "Kiphire", "Kohima", "Longleng", "Mokokchung", 
        "Mon", "Peren", "Phek", "Tuensang", "Wokha", "Zunheboto"
    ],
    odisha: [
        "Angul", "Baleswar", "Bargarh", "Bhadrak", "Bolangir", 
        "Dhenkanal", "Ganjam", "Ganjam", "Kandhamal", "Kendrapara", 
        "Kendujhar", "Khurda", "Nabarangpur", "Nuapada", 
        "Rayagada", "Sambalpur", "Subarnapur", "Sundergarh"
    ],
    punjab: [
        "Amritsar", "Barnala", "Bathinda", "Faridkot", "Fatehgarh Sahib", 
        "Fazilka", "Gurdaspur", "Hoshiarpur", "Jalandhar", 
        "Kapurthala", "Ludhiana", "Mansa", "Muktsar", 
        "Nawanshahr", "Patiala", "Rupnagar", "Sangrur", "Shaheed Bhagat Singh Nagar", 
        "Tarn Taran"
    ],
    rajasthan: [
        "Ajmer", "Alwar", "Banswara", "Baran", "Barmer", 
        "Bhilwara", "Bikaner", "Bundi", "Chittorgarh", 
        "Churu", "Dausa", "Dholpur", "Dungarpur", "Hanumangarh", 
        "Jaipur", "Jaisalmer", "Jalore", "Jodhpur", "Karauli", 
        "Nagaur", "Pali", "Rajsamand", "Sawai Madhopur", 
        "Sikar", "Tonk", "Udaipur"
    ],
    sikkim: [
        "East Sikkim", "North Sikkim", "South Sikkim", "West Sikkim"
    ],
    tamilNadu: [
        "Ariyalur", "Chennai", "Chengalpattu", "Coimbatore", "Cuddalore", 
        "Dharmapuri", "Dindigul", "Erode", "Kallakurichi", 
        "Kancheepuram", "Karur", "Krishnagiri", "Madurai", 
        "Nagapattinam", "Namakkal", "Nilgiris", "Perambalur", 
        "Pudukkottai", "Ramanathapuram", "Salem", "Sivaganga", 
        "Thanjavur", "Theni", "Thoothukudi", "Tiruchirappalli", 
        "Tirunelveli", "Tirupathur", "Tiruvallur", "Tiruvannamalai", 
        "Vellore", "Virudhunagar"
    ],
    telangana: [
        "Adilabad", "Hyderabad", "Jagtial", "Jangaon", "Jayashankar Bhupalpally", 
        "Jogulamba Gadwal", "Kamareddy", "Karimnagar", "Khammam", 
        "Mahabubnagar", "Mancherial", "Medak", "Medchal-Malkajgiri", 
        "Nalgonda", "Nizamabad", "Peddapalli", "Rajanna Sircilla", 
        "Rangareddy", "Sangareddy", "Siddipet", "Suryapet", 
        "Vikarabad", "Wanaparthy", "Warangal", "Yadadri Bhuvanagiri"
    ],
    tripura: [
        "Dhalai", "Gomati", "Khowai", "North Tripura", "Sepahijala", 
        "South Tripura", "Unakoti", "West Tripura"
    ],
    uttarakhand: [
        "Almora", "Bageshwar", "Chamoli", "Champawat", "Dehradun", 
        "Haridwar", "Nainital", "Pauri Garhwal", "Pithoragarh", 
        "Rudraprayag", "Tehri Garhwal", "Udham Singh Nagar", 
        "Uttarkashi"
    ],
    uttarPradesh: [
        "Agra", "Aligarh", "Ambedkarnagar", "Amethi", "Amroha", 
        "Auraiya", "Azamgarh", "Baghpat", "Bahraich", "Ballia", 
        "Banda", "Barabanki", "Bareilly", "Basti", "Bijnor", 
        "Budaun", "Bulandshahr", "Chandauli", "Chitrakoot", 
        "Deoria", "Etah", "Etawah", "Faizabad", "Farrukhabad", 
        "Fatehpur", "Firozabad", "Gautam Buddha Nagar", "Ghaziabad", 
        "Ghazipur", "Gonda", "Gorakhpur", "Hamirpur", "Hapur", 
        "Hardoi", "Hathras", "Jalaun", "Jaunpur", "Jhansi", 
        "Kannauj", "Kanpur", "Kaushambi", "Kushinagar", 
        "Lakhimpur Kheri", "Lalitpur", "Lucknow", "Maharajganj", 
        "Mahoba", "Mainpuri", "Mathura", "Mau", "Meerut", 
        "Mirzapur", "Moradabad", "Muzaffarnagar", "Pilibhit", 
        "Pratapgarh", "Rae Bareli", "Rampur", "Saharanpur", 
        "Shahjahanpur", "Shrawasti", "Siddharthnagar", 
        "Sitapur", "Sonbhadra", "Sultanpur", "Unnao", 
        "Varanasi"
    ],
    westBengal: [
        "Alipurduar", "Bankura", "Birbhum", "Burdwan", "Cooch Behar", 
        "Dakshin Dinajpur", "Darjeeling", "Hooghly", "Howrah", 
        "Jalpaiguri", "Jhargram", "Kalimpong", "Koch Bihar", 
        "Kolkata", "Malda", "Murshidabad", "Nadia", 
        "North 24 Parganas", "Paschim Medinipur", "Purba Medinipur", 
        "Purulia", "South 24 Parganas", "Uttar Dinajpur"
    ],
    delhi: [
        "Central Delhi", "East Delhi", "North Delhi", "North East Delhi", 
        "North West Delhi", "South Delhi", "South East Delhi", 
        "South West Delhi", "West Delhi"
    ],
    puducherry: [
        "Karaikal", "Mahe", "Puducherry", "Yanam"
    ],
    ladakh: [
        "Leh", "Kargil"
    ],
    jammuKashmir: [
        "Jammu", "Srinagar", "Doda", "Rajouri", "Poonch", 
        "Udhampur", "Reasi", "Kathua", "Samba", "Anantnag", 
        "Kulgam", "Pulwama", "Shopian", "Budgam", "Ganderbal", 
        "Baramulla", "Kupwara", "Bandipora"
    ]
};
