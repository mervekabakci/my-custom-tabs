# my-custom-tabs

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





2. **HTML & CSS & JAVASCRIPT**

Javascript ile tab örnek için klasör içerisindeki 02-html-css-javascript.html dosyasını inceleyebilirsiniz. 

Not: Javascript kullanarak bir tab yapmak istiyorsak aşağıdaki kod satırlarını sayfamıza ekleyelim.

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
        height: 300px;
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
