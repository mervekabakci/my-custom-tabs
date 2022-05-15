# my-custom-tabs
1. **HTML & CSS**
2. **HTML & CSS & JAVASCRIPT**

   **-2.1. Versiyon 1**
   
   **-2.1. Versiyon 2**
   
3. **jQuery tab örneği için dosya içerisindeki ilgili sayfaya göz atabilirsiniz.**

<------------------------------------------------------------------------------------>
1. **HTML & CSS**

Html Örnek için klasör içerisindeki 01-only-html-css.html dosyasını inceleyebilirsiniz. 

Aşağıdaki kod satırlarını da ilgili html sayfamızın içerisine <style></style> tagları içerisinde veya ilgili html sayfasına bağlı olan bir css dosyası içerisine entegre edelim.
 
       body{
            margin:0;
            background-color: #bdbdc0;
        }
        .myTabs{
            display:flex;
            flex-wrap: wrap;
            max-width: 500px;
            margin:25px auto;
            padding:25px;
        }
        .myTabs input[type="radio"]{
            display:none;
        }
        .myTabs label{
            font-family: Arial, Helvetica, sans-serif;
            font-size:14px;
            color:#3a3838;
            font-weight: bold;
            background-color:#7a7979;
            padding:10px 25px;
            cursor: pointer;
            transition:all .3s ease-in-out;
            border-bottom:5px solid #7a7979;
        }
        .myTabs label:hover{
            border-bottom:5px solid #3a3838;
            background-color:#ffffff;
        }
        .myTabs .tab{
            padding:10px 20px;
            background-color:#ffffff;
            width: 100%;
            order:1;
            display:none;
            font-family: Arial, Helvetica, sans-serif;
            text-align: justify;
        }
        .myTabs .tab h2{
            font-family: Arial, Helvetica, sans-serif;
        }
        .myTabs input[type="radio"]:checked + label{
            background-color:#ffffff;
            border-bottom:1px solid #ffffff;
        }
        .myTabs input[type="radio"]:checked + label + .tab{
            display:block;
        }


<!--------------------------------------------------------------------------------------------------> 


Aşağıdaki kod yapısını html kodunuzun içerisine entegre edelim.

    <div class="myTabs">
        <input type="radio" id="tab1" name="mytabs" checked>
        <label for="tab1">Tab 1</label>
        <div class="tab">
            <h2>Tab 1 İçerik</h2>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta, velit distinctio. Hic saepe laboriosam atque repellendus excepturi porro voluptatem                    fugiat nam repudiandae. Quae quibusdam nesciunt in provident, voluptates reiciendis rem.
            </p>
        </div>
        <input type="radio" id="tab2" name="mytabs">
        <label for="tab2">Tab 2</label>
        <div class="tab">
            <h2>Tab 2 İçerik</h2>
            <p>
               Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores pariatur vitae repudiandae sint blanditiis corrupti, suscipit aspernatur porro nam                  quas accusamus obcaecati distinctio adipisci et qui, tempora ratione aperiam molestiae eum eligendi fuga debitis delectus. Pariatur cumque nisi deserunt                commodi fugiat delectus sequi ullam dicta alias. Voluptas reprehenderit sunt nulla. Laborum modi odit voluptates corporis recusandae explicabo officia                  enim odio sit reprehenderit blanditiis quo dolores vero aliquam, quasi architecto veniam laudantium minus excepturi incidunt amet, eum nam quaerat                      exercitationem. Laudantium odit aliquid aperiam beatae, atque voluptates nesciunt! Voluptatibus sed eos, aut adipisci, laborum distinctio ipsum                        aspernatur natus,  numquam a eius.
            </p>
        </div>
        <input type="radio" id="tab3" name="mytabs">
        <label for="tab3">Tab 3</label>
        <div class="tab">
            <h2>Tab 3 İçerik</h2>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Iure, perferendis!
            </p>
        </div>
    </div>


<------------------------------------------------------------------------------------------------------->


2. **HTML & CSS & JAVASCRIPT**

Javascript ile tab örnek için klasör içerisindeki 02-html-css-javascript.html dosyasını inceleyebilirsiniz. 

Not: Javascript kullanarak bir tab yapmak istiyorsak aşağıdaki kod satırlarını sayfamıza ekleyelim.

**2.1. Versiyon 1**

İlgili Css Kodu

    body{
        background-color:rgb(196, 192, 192);
    }
    .myTabs{
        max-width: 500px;
        margin:25px auto;
    }
    .myTabs .tabsContent{
        font-family:Arial, Helvetica, sans-serif;
        width:100%;
    }
    .myTabs .tabsTitle .tabButton{
        background-color:gray;
        font-family: 'Arial';
        color:white;
        font-size:16px;
        text-decoration: none;
        padding:10px 25px;
        outline:none;
        border:none;
        cursor: pointer;
        display: inline-block;
    }
    .myTabs .tabsTitle .tabButton.active{
        background-color:#ffffff;
        color:gray;
    }
    .myTabs .tabsContent .tabContent{
        padding:10px 20px;
        display:none;
        font-size: 14px;
        background-color:#ffffff;
        height: auto;
    }
    .myTabs .tabsContent .tabContent:first-child{
        display:block;
    }


<!----------------------------------------------------------------------------->

İlgili Html kodu
 
    <div class="myTabs">
        <div class="tabsTitle">
            <label class="tabButton active" id="tabBttn1" onclick="myTabSelector('tab1', this.id)">Tab 1</label>
            <label class="tabButton" id="tabBttn2" onclick="myTabSelector('tab2', this.id)">Tab 2</label>
            <label class="tabButton" id="tabBttn3" onclick="myTabSelector('tab3', this.id)">Tab 3</label>
        </div>
        <div class="tabsContent">
            <div id="tab1" class="tabContent">
                <h2>Tab Content 1</h2>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur, ex. Dolorum corporis deserunt laboriosam culpa maxime cum suscipit magni, accusamus dolor ad incidunt aperiam eligendi iste ex voluptatum sit facilis eaque. Soluta quis alias officia sequi id consequatur inventore expedita culpa atque vitae odit officiis maxime, enim nihil magni recusandae maiores nulla ullam, cupiditate ipsa aliquam tenetur itaque! Reprehenderit, nemo possimus, facilis soluta eveniet iure vel nihil odit earum illum officia illo delectus consectetur perferendis error incidunt vero et sunt eos. Hic, atque laborum, voluptate totam deleniti non rerum porro quae iusto eos libero quasi sit consequatur animi expedita est?
                </p>
            </div>
            <div id="tab2" class="tabContent">
                <h2>Tab Content 2</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Natus debitis mollitia inventore sequi sint suscipit ex sunt aspernatur numquam neque consectetur ducimus, libero distinctio rerum tenetur quae aliquam ipsam eum nobis, praesentium accusantium nemo. Voluptatem vero omnis doloribus, quod sunt iure dolore, commodi tempora, fugit nobis molestiae totam tempore nemo.</p>

            </div>
            <div id="tab3" class="tabContent">
                <h2>Tab Content 3</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis tempore esse quo rem, earum ratione reiciendis nam quidem eveniet quos, veritatis pariatur inventore aliquam, minima vel commodi atque! Dolor eligendi accusantium reprehenderit atque, recusandae deserunt unde assumenda laborum eaque quis fugit doloremque molestiae officiis, ex fuga harum reiciendis vitae consectetur obcaecati cum, adipisci asperiores quod? Rem hic est recusandae nobis assumenda tempore et fugit veniam praesentium. Quis pariatur voluptates error doloribus in libero et id, architecto ipsum fuga magni ea, laudantium velit. Magni, eligendi. Odio perferendis, unde esse dolorem ratione minus nostrum quam culpa, soluta debitis quia cumque a officia ipsam numquam quas reprehenderit labore exercitationem, totam voluptatum quisquam accusamus autem alias! Provident, voluptates earum eaque vel ad reiciendis voluptatum voluptas laborum eius consectetur ex praesentium eveniet, laboriosam accusamus incidunt! Nemo sed harum consequatur eos fugit facilis laborum? Saepe omnis quas eveniet voluptas rem aliquam labore, dicta quibusdam laudantium animi.</p>
            </div>
        </div>
    </div>
    
    
    
<!------------------------------------------------------------------------------------------>
 
 İlgili Javascript kodu
  
       /*Seçili içerik alanın açılması*/
        function myTabSelector(deger,tabId){
            allTabContentHide();
            document.getElementById(deger).style.display = "block";
            selectedTabBttn(tabId);
        }

        /*Tüm İçerik alanlarının silinmesi*/
        function allTabContentHide(){
            const tabs = document.querySelector(".tabsContent");
            const alanlar = tabs.querySelectorAll("div.tabContent");
            for (var baslangic = 0; baslangic < alanlar.length; baslangic++){
                alanlar[baslangic].style.display = "none"; 
            }
        }

        /*Seçili butonun aktif olma özelliği verilmesi*/
        function selectedTabBttn(tabId){
            var tabButtons= document.getElementsByClassName("tabButton");
            for (var baslangic = 0; baslangic < tabButtons.length; baslangic++){
                tabButtons[baslangic].classList.remove("active")
            }
            document.getElementById(tabId).classList.add("active");
        }
        
<--------------------------------------------------------------------------------------------------------------------------->

**2.1. Versiyon 2**

    *{
        box-sizing: border-box;
    }
    body{
        background-color:#c4c0c0;
    }
    h2{
        font-family: Arial, Helvetica, sans-serif;
    }
    .myTabs{
        max-width: 500px;
        margin:25px auto;
    }
    .tabButton{
        background-color:gray;
        font-family: 'Arial';
        color:white;
        font-size:16px;
        text-decoration: none;
        padding:20px 25px;
        outline:none;
        border:none;
        float: left;
        width: 25%;
        cursor: pointer;
        transition:all .3s ease-in-out;
        border-left:1px solid lightgray;
    }
    .tabButton:first-child{
        border-left:none;
    }
    .tabButton:hover{
        background-color:#686262;
    }
    .tabContent{
        padding:70px 20px 20px;
        font-size: 14px;
        background-color:#ffffff;
        height: auto;
        display: none;
        font-family: Arial, Helvetica, sans-serif;
    }
    .tabContent p{
        text-align: justify;
    }


<!-------------------------------------------------------------------------------------------------->

 <!--Tab Button Oluşturma-->
    <button id="defaultOpen" class="tabButton" onclick="openTab('tab1', this)">Tab 1</button>
    <button class="tabButton" onclick="openTab('tab2', this)">Tab 2</button>
    <button class="tabButton" onclick="openTab('tab3', this)">Tab 3</button>
    <button class="tabButton" onclick="openTab('tab4', this)">Tab 4</button>

    <!--Tab İçerik alanı olusturma-->
    <div id="tab1" class="tabContent">
        <h2>Tab 1 İçerik</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum, porro eius pariatur beatae velit harum error enim, tempore non labore, nostrum ea asperiores quaerat itaque vero aliquam! Dolorem maxime quasi ad unde minus aut minima, iste repellat similique harum placeat ipsam ut consequuntur id, pariatur ea veritatis maiores blanditiis tempore. Neque deleniti quas libero reprehenderit distinctio, maxime atque placeat iusto dolorum unde eum minima ratione obcaecati molestias, rem, fuga veniam perferendis laborum corrupti sint suscipit debitis. Sequi vel voluptas ipsam harum architecto reprehenderit repudiandae, distinctio totam natus eos, nostrum mollitia non voluptatum accusantium veniam sapiente, minima ullam? Eaque, laboriosam praesentium?</p>
    </div>
    <div id="tab2" class="tabContent">
        <h2>Tab 2 İçerik</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus, fugit sint ab voluptatum esse dolores adipisci, itaque ipsa repudiandae qui iste aspernatur atque asperiores, eius possimus deleniti quod. Eius repudiandae temporibus id voluptates ab quidem maiores aut eligendi similique ad, autem molestias pariatur architecto obcaecati doloribus, modi veritatis culpa hic perspiciatis! Adipisci libero eveniet, voluptas iusto cumque dignissimos sequi consequuntur impedit consectetur error vitae voluptates reiciendis velit laudantium sunt fuga mollitia. Impedit, ut reiciendis nesciunt distinctio officia hic cumque in ullam, ducimus fugit repudiandae sint quidem similique. Ut veritatis distinctio labore repellendus nisi sapiente, aliquid accusamus quam. Natus ipsam quasi earum minus voluptate. Iure aut totam fugit numquam distinctio qui quibusdam fuga assumenda perspiciatis consectetur commodi ad voluptas eveniet non porro, reprehenderit et at corrupti ipsam molestiae debitis ea nisi accusamus? Eveniet laudantium eos repellendus rerum corporis expedita non itaque veritatis tempora excepturi deserunt cum quo odio, ut et ipsam mollitia. Obcaecati quis deleniti perspiciatis consectetur culpa cumque maxime optio accusamus sit iste ipsam dicta ab pariatur fuga nisi, maiores saepe natus autem magni ex alias rem dolor architecto. Odit accusantium eveniet quibusdam impedit excepturi maiores fugiat repudiandae tempora, saepe amet ad sit rerum veniam nostrum consequatur pariatur sunt, ducimus vel ipsam! Fugit nostrum nam autem vel quos possimus ea debitis aperiam enim optio, quaerat maxime fuga saepe soluta beatae, dolorum esse. Unde ipsum vitae voluptatum perspiciatis eos eius tenetur adipisci mollitia in. Inventore obcaecati perspiciatis natus dolor dicta, illo similique error a eos repudiandae doloremque cumque, aspernatur itaque? Nemo, perferendis nam repellat ab dignissimos non facere nihil voluptatum vitae fugiat tempora corporis facilis praesentium mollitia dolores amet illum laudantium explicabo voluptatem eveniet? Ipsam vero vitae rerum, ex dolor debitis pariatur id neque tenetur necessitatibus voluptate asperiores cupiditate a obcaecati distinctio iusto quae doloribus alias? Fugit doloremque tempora earum culpa.</p>
    </div>
    <div id="tab3" class="tabContent">
        <h2>Tab 3 İçerik</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum, porro eius pariatur bea</p>
    </div>
    <div id="tab4" class="tabContent">
        <h2>Tab 4 İçerik</h2>
        <p>Lorem ipsum dolor sit amet mollitia non voluptatum accusantium veniam sapiente, minima ullam? Eaque, laboriosam praesentium?</p>
    </div>
    
<!-------------------------------------------------------------------------------------------------->
    <!--Javascript tab Menu Javascript start-->
    <script type="text/javascript" language="javascript">
        function openTab(tabId, elemnt) {
            var i, tabContent, tabButton;

            /*Tüm İçerik alanlarını gizleme*/
            tabContent = document.getElementsByClassName("tabContent");
            for( var i = 0; i < tabContent.length; i++){
                tabContent[i].style.display="none";
            }

            /*Tab butonun arkaplan rengini silme*/
            tabButton = document.getElementsByClassName("tabButton");
            for(var i =0; i < tabButton.length; i++){
                tabButton[i].style.backgroundColor ="";
            }

            /*Seçili içerik alanını gösterme ve seçili tab buttonuna özellik verme*/
            document.getElementById(tabId).style.display="block";
            elemnt.style.backgroundColor="#504f4f";

        }
        /*Sayfa açıldıgında açık gelen ilk tab*/
        document.getElementById("defaultOpen").click();
    </script>
   
