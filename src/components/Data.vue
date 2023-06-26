<template>
    <div id="Userinfo"></div>
</template>

<script>
async function Userdata() {
    const data = await fetch(
        "https://laiquah.github.io/jsonserver/server.json"
    );
    const jsonData = await data.json();
    console.log(jsonData);
    let peopleData = jsonData.students;
    const display = document.querySelector('#Userinfo');

    peopleData.forEach((data) => {
        display.innerHTML += `
        <div class="card m-4 shadow">
        <div class="card-body">
            <h3 class="card-title">${data.first_name} ${data.last_name}</h3>
            <p class="card-text">${data.email}</p>
            </div>
        </div>
        `;
    })
}
Userdata();
</script>

<style scoped></style>