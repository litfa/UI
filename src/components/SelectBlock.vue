<!--
  Copyright (C) 2022 Suwings <Suwings@outlook.com>

  This program is free software: you can redistribute it and/or modify
  it under the terms of the GNU Affero General Public License as published by
  the Free Software Foundation, either version 3 of the License, or
  (at your option) any later version.
  
  According to the AGPL, it is forbidden to delete all copyright notices, 
  and if you modify the source code, you must open source the
  modified source code.

  版权所有 (C) 2022 Suwings <Suwings@outlook.com>

  该程序是免费软件，您可以重新分发和/或修改据 GNU Affero 通用公共许可证的条款，
  由自由软件基金会，许可证的第 3 版，或（由您选择）任何更高版本。

  根据 AGPL 与用户协议，您必须保留所有版权声明，如果修改源代码则必须开源修改后的源代码。
  可以前往 https://mcsmanager.com/ 阅读用户协议，申请闭源开发授权等。
-->

<template>
  <div class="select-block" :style="style">
    <div>
      <p class="color-black" style="font-size: 14px; font-weight: 600; letter-spacing: -0.4px">
        <slot name="title"></slot>
      </p>
      <p class="sub-title">
        <slot name="info"></slot>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    style: String
  },
  data: function () {
    return {};
  },
  methods: {}
};
</script>

<style scoped>
.select-block {
  border: 1px solid #dcdfe6;
  cursor: pointer;
  border-radius: 4px;
  overflow: hidden;
  transition: all 0.4s;
  padding: 4px 14px;
}

.select-block:hover {
  border: 1px solid #409eff;
}

.sub-title {
  color: gray;
  font-size: 13px;
}
</style>
