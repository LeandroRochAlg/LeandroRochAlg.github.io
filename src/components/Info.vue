<script setup lang="ts">

</script>

<template>
    <div class="info">
        <code>
            <div class="item">
                <span class="variableName">age:</span>
                <p><span class="variableValue">"21"</span></p>
            </div>
            <div class="item">
                    <span class="variableName">education:</span>
                <div>
                    <p><span class="variableValue">"Building Construction"</span>,</p>
                    <p><span class="variableValue">"Computer Science"</span></p>
                </div>
            </div>
        </code>
    </div>
</template>

<style scoped>
  .info{
    text-align: left;
  }

  .variableName{
    color: #FFD700;
  }

  .variableValue{
    color: #00FF00;
    margin-left: 2rem;
  }
</style>