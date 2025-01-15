**My Review regarding your web page**

Why did you use classes instead of id as there is no duplicacy of tags except p tag ?
```bash
<div
      class="greet-container"
      style="
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        border: 1px solid #fff;
        padding: 20px;
        border-radius: 10px;
        background-color: #000;
        "
    >
      <h1 style="
      color: #bcbec0; 
      font-size: 50px
      ">
The greeting zone
🎊
      </h1>
      <p 
      style="
      font-size: 25px;
      color: #fff;
      ">
     Click here to receive your greeting
    </p>

      <button
        class="greet-btn"
        style="
          background-color: #1f1e1e;
          color: #fff;
          border: none;
          padding: 10px;
          border-radius: 5px;
          cursor: pointer;
          font-size: 20px;
        "
      >
        Greet
      </button>

      <p
        class="greet-message"
        style="
        display: none; 
        font-size: 30px;
        color: #ffffff;
        "
      >
      Sat shri akaal! Have a good day.
      <button 
      class="back-btn"
      style="background-color: #1f1e1e;
      color: #fff;
      border: none;
      padding: 10px;
      border-radius: 5px;
      cursor: pointer;
      font-size: 20px;">Hide</button>
      </p>
    </div>
```
2)
```bash
<button
        class="greet-btn"
        style="
          background-color: #1f1e1e;
          color: #fff;
          border: none;
          padding: 10px;
          border-radius: 5px;
          cursor: pointer;
          font-size: 20px;
        "
      >
        Greet
      </button>
```
Suggestion:-
Border should be changed to solid one .Its my  choice anyways but if you want to add border so it should be removed as border radius is already given and show its effect

3)
```bash
<script>
      const button = document.querySelector(".greet-btn");
      const back = document.querySelector(".back-btn");
      button.addEventListener("click", () => {
        const message = document.querySelector(".greet-message");
        message.style.display = "block";
      });
      back.addEventListener("click", ()=>{
        location.reload()
      })
    </script>
```
Suggestion-Why haven't you use  toggle button for hiding the greet message instead you have used location.reload() as it render extra refreshing the entire page along
                with other content ?



