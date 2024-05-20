function showContent(id) {
  var contents = document.querySelectorAll(".content");
  contents.forEach((content) => content.classList.remove("active"));

  var activeContent = document.getElementById(id);
  activeContent.classList.add("active");

  if (id === "chatboxContent") {
    document.body.classList.add("no-scroll");
  } else if (id === "loginContent") {
    document.body.classList.add("no-scroll");
  } else if (id === "signupContent") {
    document.body.classList.add("no-scroll");
    document.body.classList.add("bg-yellow_body");
  } 
  else if (id === "blogContent" || id === "exerciseContent"  || id === "aboutContent"  || id === "pricingContent") {
    document.body.classList.add("bg-black");
    document.body.classList.add("no-scroll");
  }else {
    document.body.classList.remove("no-scroll");
    document.body.classList.remove("bg-black");
  }
}