<template>
    <div id="formHead">
        <h1>Contineous Assessment Form</h1>
        <div id="formInner">
            <label for="">class: 
                <select name="" id="">
                    <option value="2A1">2A1</option>
                    <option value="2A4">2A4</option>
                    <option value="2A7">2A7</option>
                    <option value="2S1">2S1</option>
                    <option value="2S3">2S3</option>
                </select>
            </label>
            <label for="">Assessment Type:
                <select name="" id="Assessment">
                    <option value="male">Home Work</option>
                    <option value="female">Excecise</option>
                    <option value="female">Project Work</option>
                    <option value="female">Class Test</option>
                </select> 
            </label>
            <label for="">
                Total Mark: <input type="text" name="" id="">
            </label>
            <label for="">Term:
                <select name="" id="term">
                    <option value="first">First</option>
                    <option value="second">Second</option>
                    <option value="third">Third</option>
                </select>
            </label>
        </div>
    </div>
</template>


<script>

export default {
    name: "formHead",
}
</script>


<style scoped>
    #formHead {
        margin: 0;
        background-color: blueviolet;
        text-align: center;
    }

    h1 {
        text-align: center;
    }

    #formInner {
        display: grid;
        grid-template-columns: 25% 25% 25% 25%;
        font-size: 1.5rem;
        text-align: center;
    }

</style>