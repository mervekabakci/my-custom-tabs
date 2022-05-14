# my-custom-tabs / html&css

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


 
